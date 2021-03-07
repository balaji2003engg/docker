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

Remove all unused containers, networks, images (both dangling and unreferenced), and optionally, volumes.
      REflink : https://docs.docker.com/engine/reference/commandline/system_prune/
      $ docker system prune

          WARNING! This will remove:
               - all stopped containers
               - all networks not used by at least one container
               - all dangling images
               - all build cache

Volumes and Port Mapping
 Run the docker  container of nginx image with port 81 and point out the volume of local machine to container
 
      docker run -d -p 81:80 -v /root/mynginx:/usr/share/nginx/html nginx
       
       (docker run -d -p hostport:conatinerport -v hostmachinepath:conatinerpath dockerimage)
      
      
 



    
