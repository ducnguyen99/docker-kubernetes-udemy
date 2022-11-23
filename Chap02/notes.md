- create image: `docker create <image_name>`
- run image without output: `docker start <image_name>`
- run image with output: `docker start -a <image_name>`
- create and run image: `docker run <image_name>`

- run startup command in image: `docker run <image_name> <command>` 

- list all running containers:  `docker ps`
- list all containers:  `docker ps --all`

- restart image output: `docker start <container_id>`

- remove stopped containers: `docker system prune`
- retriving log outputs: `docker logs <container_id>`
- stop containers: `docker stop <container_id>`
- kill containers: `docker kill <container_id>` 
- execute command in a container: `docker exec -it <container_id> <command>`

**Note:** -it = -i -t 
- -i = allow to take input argument
- -t = make text shown in a nice format

- go to container shell: `docker exec -it <container_id> sh` **or** `docker exec -it <image_name> sh` 

- attach volumes: `docker run -v $(pwd):/app <image_id>`

- attach volumes with bookmark folder: `docker run -v /app/node_modules -v $(pwd):/app <image_id>`
