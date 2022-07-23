# Introduction to Containers, Kubernetes, and OpenShift

## Module 1 Cheat Sheet: Understanding the Benefits of Containers

> The Docker CLI

Command Description

docker build = Builds an image from a Dockerfile.
docker CLI = Start the Docker command line interface.
docker container rm = Removes a container.
docker images = Lists the images.
docker ps = Lists the containers.
docker pull = Pulls the latest image or repository from a registry.
docker push = Pushes an image or a repository to a registry.
docker run = Runs the <image name> in a new container.
docker run = Runs a command in a new container.
docker stop = Stops one or more running containers.
docker tag = Creates a tag for a target image that refers to a source image.

> You can refresh your understanding of the commands mentioned in the Dockerfile below:

1. The FROM instruction initializes a new build stage and specifies the base image that subsequent instructions will build upon.
2. The COPY command enables us to copy files to our image.
3. The RUN instruction executes commands.
4. The EXPOSE instruction exposes a particular port with a specified protocol inside a Docker Container.
5. The CMD instruction provides a default for executing a container, or in other words, an executable that should run in your container.

# Module1 Glossary: Understanding teh Benefits of Containers

1. Container == An executable unit of software in which application
   code is packaged, along with its libraries and
   dependencies, in common ways so that it can be run
   anywhere, whether on a desktop, on-premises, or in the
   cloud

2. Container Registry = Used for the storage and distribution of named
   container images. While many features can be built on
   top of a registry, its most basic function is storing
   images and allowing someone to later retrieve them.

3. Docker = A software platform for building and running
   applications as containers.

4. DockerFile = A blueprint from which an image is built. It outlines
   all the steps to be taken to build the desired image;
   Docker then builds that image. A Dockerfile is a text
   file that contains all the commands a user would call
   on the command line to create the image.

5. Image = An immutable file that contains the source code,
   libraries, and dependencies that are necessary for an
   application to run. Images are templates or blueprints
   for a container.

6. Private Registry = Restricts access to images so that only authorized
   users can view and use them.

7. Tag = Provides information about a specific version or
   variant of an image. The tag is often a version number,
   or indicate some other characteristic of the
   image, such as the operating system on which it was
   built.
