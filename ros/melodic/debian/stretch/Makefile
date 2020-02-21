all: help

help:
	@echo ""
	@echo "-- Help Menu"
	@echo ""
	@echo "   1. make build            - build all images"
	@echo "   2. make pull             - pull all images"
	@echo "   3. make clean            - remove all images"
	@echo ""

build:
	@docker build --tag=ros:melodic-ros-core-stretch-no-recommends          ros-core/.
	@docker build --tag=ros:melodic-ros-base-stretch-no-recommends          ros-base/.
	@docker build --tag=ros:melodic-robot-stretch-no-recommends             robot/.
	@docker build --tag=ros:melodic-perception-stretch-no-recommends        perception/.
	# @docker build --tag=osrf/ros:melodic-desktop-stretch      desktop/.
	# @docker build --tag=osrf/ros:melodic-desktop-full-stretch desktop-full/.

pull:
	@docker pull ros:melodic-ros-core-stretch-no-recommends
	@docker pull ros:melodic-ros-base-stretch-no-recommends
	@docker pull ros:melodic-robot-stretch-no-recommends
	@docker pull ros:melodic-perception-stretch-no-recommends
	# @docker pull osrf/ros:melodic-desktop-stretch
	# @docker pull osrf/ros:melodic-desktop-full-stretch

clean:
	@docker rmi -f ros:melodic-ros-core-stretch-no-recommends
	@docker rmi -f ros:melodic-ros-base-stretch-no-recommends
	@docker rmi -f ros:melodic-robot-stretch-no-recommends
	@docker rmi -f ros:melodic-perception-stretch-no-recommends
	# @docker rmi -f osrf/ros:melodic-desktop-stretch
	# @docker rmi -f osrf/ros:melodic-desktop-full-stretch
