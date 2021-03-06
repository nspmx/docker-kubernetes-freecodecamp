# docker-kubernetes-freecodecamp
My personal project folder for the course Docker and Kubernetes by freeCodeCamp.org

## Important Links

- [YouTube Course](https://www.youtube.com/watch?v=Wf2eSG3owoA)
- [Docker Docs](https://docs.docker.com/get-started/)
- [Docker Hub](https://hub.docker.com/)
- [expressjs](https://expressjs.com/)

## Notes

### Docker

- Tool for running applications in an isolated Environment (Similar to a VM)
- Apps run in the same environment in wathever machine that you could use
- Registry: place where you can download images

### Container VS Virtual Machines

Containers are an abstraction at the app layer that **packages code and dependencies** together. **Multiple** containers can run on the **same machine** and share the OS kernel with other containers, each running as isolated processes in user space. Containers doesn't required an operative systems.

Virtual Machines are an abstaction of physical hardware turning **one server** into **many servers**. You can ran multiple VMs on a single machine, but **every VM includes a full copy of an operating system**, the application, the necessary binaries and the libraries required.

![container-vs-vms](/images/container-vs-vms.jpg)

#### Benefits:
- Boots up quickly than a VM
- Usses less memory and less disk memory
- Does not need a full operative system
- Deployment and testing 

### Docker Image

A Docker Image is a **template** for creating an **environment** of your choice, it has everything that the app needs to run, os, software, app code, everything.

Also, you can have **multiple versions** of a docker image, meaning that it can be used also as a snapshot for different versions of an app.

### Docker Container

A Docker Container it's a running instance of a Docker Image.

### Docker Volumes

Volumes allow sharing data (folders and files) in between host and container or two or more containers.

![mount-volumes](/images/mount-volumes.png)

### Dockerfile

Used to build our own images. List of steps of how to create images

- [Dockerfile Reference](https://docs.docker.com/engine/reference/builder/)
- [Dockerfile Best Practices](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/)

#### .dockerignore

#### Caching and Layers

#### Alpine

Check alpine version of images for lightweight versions.

#### Tags and Versions

Allows controll for image version

### Docker Registry

Highly scalable server side application that stores and lets you distribute Docker images. Use it for CI/CD or running applications.

#### Private / Public

#### Most used registry sites
- [Docker Hub](https://hub.docker.com/)
- [Amazon ECR](https://aws.amazon.com/ecr/)
- [quay.io](https://quay.io/)

### Docker Inspect

Displays information about a container

### Docker Logs

### Docker Exec

Get into the container