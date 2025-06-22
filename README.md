# turtlebot4-playground

This repository hosts a ROS 2 workspace used for experimenting with the TurtleBot 4 stack.

## Workspace layout

The workspace lives under `tb4_ws/` and imports the upstream TurtleBot 4 packages
listed in `dependencies.repos` on the `humble` branches.

## Container

A `docker/Dockerfile` is provided to build the workspace using the
`gz-harmonic:2025-05` base image with ROS 2 build tools installed.

## Continuous Integration

GitHub Actions runs `colcon test` followed by a simple Gazebo smoke test
whenever a change is pushed or a pull request is opened.
