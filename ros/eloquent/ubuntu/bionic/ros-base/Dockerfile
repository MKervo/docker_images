# This is an auto generated Dockerfile for ros:ros-base
# generated from docker_images_ros2/create_ros_image.Dockerfile.em
FROM ros:eloquent-ros-core-bionic-no-recommends

# install packages
RUN apt-get update && apt-get install -q -y --no-install-recommends \
    build-essential \
    && rm -rf /var/lib/apt/lists/*

# install ros2 packages
RUN apt-get update && apt-get install -y --no-install-recommends \
    ros-eloquent-ros-base=0.8.4-1* \
    && rm -rf /var/lib/apt/lists/*

