# docker

Docker Run the image in the backend

      docker run -d hello-world

Enter into the docker container

     docker exec -it containerid /bin/bash
     
Docker inspect to show full information of docker container

    docker inspect containerid
    
To show all the containers which include exited containers

    docker ps -a
 
 Push image to the docker hub
 
    1. docker login ( Provide the dockerhub username and password)
    2. docker tag balaji2003engg/myimage:1.2   ( docker tag accountid/imagename:version)
    3. docker push balaji2003engg/myimage:1.2

Run the docker hub image into the container

      docker run -d balaji2003engg/myimage:1.2

Delete the images

      docker rmi -f dockerimageid
      
 Delete the containers
 
     docker rm -f containerID
     
     
  
    
