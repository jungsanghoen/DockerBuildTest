# dockerfiles-ubuntu-user-adderable
Ubuntu, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build   --rm -t jusahe/ubuntu_git:4 .
	docker run -it --rm --name u1  jusahe/ubuntu_git:4
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE                COMMAND             CREATED             STATUS              PORTS               NAMES
63a0ba73bf81        jusahe/ubuntu:4   "/bin/bash"         4 seconds ago       Up 3 seconds                            u1
```

To test,
```
	tree
```
To Rollback
```
    docker rm u1 -f 
    docker rmi jusahe/ubuntu:test
```

update