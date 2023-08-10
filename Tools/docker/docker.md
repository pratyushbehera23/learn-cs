# Docker

A platform for building, running and shipping applications in a consistent manner along any machine.

With Docker we can package up our application with everything it needs and run it anywhere on any machine with Docker.
All dependencies will be included in the application package, this package helps running on any machine. Docker will run these dependencies inside an isolated environment called a container.
these isolated environment helps run multiple applications with different versions of some software side by side.

## Virtual machines vs Containers

### VM

Virtual machine is an abstraction of a machine or physical hardware, so we can run several VMs on a real machine, hence run our applications in isolation.
Hypervisor a software use to create and manage VMs.  ex: VirtualBox, VMware, HyperV ..
Problems: Each VM needs a full OS of its own, slow to start, resource intensive.

### Containers

Containers give us same kind of isolation; but lightweight, fast, need less hardware resource, dont need a full OS (share OS(kernel) of the host)

## Architecture of Docker

Docker uses a Client Server Architecture
It has a client component that talks to a server component using a REST API.
The server also called the docker engine, sits in the background and takes care of building and running docker containers.

## Installing Docker

docs.docker.com

> docker version
    Client
    Server
> Development workflow

Add a Dockerfile to your application.
A Dockerfile is a plain text file that includes instructions that docker uses to package up this application into an image; This image contains everything our application needs to run.
Image contains cut-down OS, a runtine environment (eg. Node), app files, libraries, env variables, ..

We created a Dockerfile and give it to docker for packaging our application into an image.
Once we have an image, we tell docker to start a container using that image.
So, a container is just like a process running on your computer, but its a special kind of process as it has its own file system provided by the image.
So, our application gets loaded inside a container/process, this is how we run our app locally on our development machine.

> docker run ..

Once we have this image, we can push it to a docker registry like DockerHub, a storage for docker images that anyone can use.

hub.docker.com

Open a folder inside vscode
...your app code
Add a file with just name "Dockerfile" no extension
Write instructions for packaging the image here

## FROM linux

```Dockerfile
FROM node:alpine  
# (alpine linux becz very small image)
COPY . /app  
# copy all programs from this folder to a docker folder (as named 'app' here)
WORKDIR /app  
# makes work directory to app folder
CMD node app.js  
# run this command
# or
CMD node /app/app.js  
# if not set WORKDIR
```

```sh
docker build -t app-name .  (. becz current folder)
docker image ls   /   > docker images
docker run app-name
docker pull yourDockerhubusername/app-name
docker image ls
docker run yourDockerhubusername/app-name
docker pull ubuntu  /  > docker run ubuntu
docker ps
docker ps -a
docker run -it ubuntu
root@2f578e6756e7:/#
(root @2f578e6756e7 : / # )
```
