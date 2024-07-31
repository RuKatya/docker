# Docker
## Info
* ```:latest``` = the latest version of image.

## PowerShell Comands 
* ```ls``` = show folders and files in the current folder
* ```ls -la``` = show folders and files in the current folder (with hidden folders and files)
* ```hostname``` = show name of the container/computer
* ```ping _ip adress_/_domain_``` = check if the computer/computer have internet connect
* ```cd [folder-name]```= navigate to the folder.
* ```cat [file-name]``` = get content of the file.

## Docker Comands
* ```docker ps``` = show all working containers
* ```docker ps -a``` = show all containers
* ```docker images``` = show local images
* ```docker run [image-name]``` = create and run container. If the image did not exist localy, docker check it from docker hub. 
* ```docker **pull** [image-name]``` = download image
* ```docker rm [container id]/[name]``` = remove container
* ```docker run -it(interactive terminal) [image-name]``` = run and conntect to the container with option interactive in the container.
* ```hostname -i``` =  show ip adress of the container/computer
* ```exit``` = stop running container
* ```docker container prune``` = remove all stopped containers
* ```docker run -d [image-name]``` = run in background
* ```docker container inspect [container id]/[name]``` = show all details of a container.
* ```docker container **inspect** [container id]/[name] | grep [IPAddress]``` = filter the details of a container and show IPAddress.
* ```docker stop [container id]/[name]``` = stop the container.
* ```docker kill [container id]/[name] ```= stop the container immediately.
* ```docker exec -it [container id]/[name] bash```= run comand in already running container with name of process.
* ```docker run -d --name [name-of-image]``` = create a container with a custom name.
* ```docker run -p [8080]:[80] [name-of-image]``` = Creating and running a container on custom post (external port:container port).
* ```docker run -v ${PWD}:[/usr/share/nginx/html] nginx``` = Creating and running a container with connecting volume to the local path to the html file. 
* ```docker run -it --rm [busybox]``` = remove container after stop
* ```docker run \--name [my-doc] \-p 8888:80``` = with \ symbol with can start new row.

## Images 
* [hello-world](https://hub.docker.com/_/hello-world)
* [busybox](https://hub.docker.com/_/busybox)
* [nginx](https://hub.docker.com/_/nginx)
