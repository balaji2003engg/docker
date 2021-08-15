#docker-compose

Docker compose installation

Ref link : https://docs.docker.com/compose/install/

    sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    sudo chmod +x /usr/local/bin/docker-compose
    

Docker compose Build (Create the image of using dockerfile with docker-compose)

Below command will build the dockerfile and create the docker image

     docker-compose build
     
Create the containers with docker compose

    docker-compose up -d
    
Push image to the docker hub

    docker-compose push
  
 scale the docker contianers
 
     docker-compose up -d --scale redis =2
     
     (docker-compose i -d --scale NameOfImageInDockercompose= number)
