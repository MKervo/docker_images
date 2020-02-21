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
	@docker build --tag=ros:eloquent-ros-core-bionic-no-recommends			ros-core/.
	@docker build --tag=ros:eloquent-ros-base-bionic-no-recommends			ros-base/.
	# @docker build --tag=osrf/ros:eloquent-desktop-bionic			desktop/.
	# @docker build --tag=osrf/ros:eloquent-ros1-bridge-bionic			ros1-bridge/.

pull:
	@docker pull ros:eloquent-ros-core-bionic-no-recommends
	@docker pull ros:eloquent-ros-base-bionic-no-recommends
	# @docker pull osrf/ros:eloquent-desktop-bionic
	# @docker pull osrf/ros:eloquent-ros1-bridge-bionic

clean:
	@docker rmi -f ros:eloquent-ros-core-bionic-no-recommends
	@docker rmi -f ros:eloquent-ros-base-bionic-no-recommends
	# @docker rmi -f osrf/ros:eloquent-desktop-bionic
	# @docker rmi -f osrf/ros:eloquent-ros1-bridge-bionic
