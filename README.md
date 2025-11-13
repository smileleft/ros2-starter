# ros2-starter
repository for ros2 startup

## ros2 github
https://github.com/ros2

## ros2 document
https://docs.ros.org/en/foxy/index.html

## run ros2 with docker
```
# pull ros2 docker image with tag "foxy-desktop"
docker pull osrf/ros:foxy-desktop

# run the image in a container in interactive modde
docker run -it osrf/ros:foxy-desktop

# check
root@<container-id>:/# ros2 --help
```

## run 2 nodes in two seperate docker containers
```
# run talker
docker run -it --rm osrf/ros:foxy-desktop ros2 run demo_nodes_cpp talker

# run listener
docker run -it --rm osrf/ros:foxy-desktop ros2 run demo_nodes_cpp listener
```
