# A Beginner's Guide to Docker

A way to isolate and run applications

## Linux Containers

Docker is really just Linux containers
- Virtual Machine: Copies of a computer system from the operating system on up
- Fundamentally, Docker is a way to implement Linux containers

## Containers vs Virtual Environments

Virtual environments isolate Python software packages locally
- can only isolate Python packages
- can't run a production database or other services within a virtual environment

## Images and Containers

An image is a snapsot of what a project contains
- a container runs an instance of the image
- Dockerfile is a list of instructions for creating an image
