## Signal Sciences Docker Configuration - Ubuntu 16.04

This is a dockerized SigSci Agent to be used as a side car or as a reverse proxy running on Ubuntu 16.04. You can use a pre-built container or build your own. When building and deploying I tend to use OS version followed by the agent type for the container name.


## Information about the files

**start.sh**
The start.sh is a simple script for doing some customizations. I use it to start the SigSci agent process.  

**Dockerfile**
The included dockerfile is my example for creating a container that has the SigSci Agent installed running on Golang distributed Alpine Linux.

**Makefile**
I tend to prefer nice easy command for doing my tasks in building, deploying, and testing locally. The makefile simplifies this process but is not necessary. I edit this file for each build and run I need to but you can change it to accept environment variables so you can pass dynamic content in the make statements.

## Building Docker image

make build

## Running the container

make run
