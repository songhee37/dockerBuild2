# dockerBuild2
# dockerfiles-ubuntu-user-adderable
Ubuntu, It support base user creation and password setting.
# added line by hyeonjae-J

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build   --rm -t shlee719/ubuntu:test .
	docker run -it --rm --name u1  shlee719/ubuntu:test
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE                COMMAND             CREATED             STATUS              PORTS               NAMES
63a0ba73bf81        shlee719/ubuntu:test   "/bin/bash"         4 seconds ago       Up 3 seconds                            u1
```

To test,
```
	tree
```
To Rollback
```
    docker rm u1 -f 
    docker rmi shlee719/ubuntu:test
```
