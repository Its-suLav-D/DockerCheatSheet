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

# Container Orchestration (Kubernetes)

> Manage the lifecycle of container, espscially in large, dynamic enviornments

1. Provisioning and deployment
2. Availability
3. Scaling
4. Scheduling to Infrastructure
5. Rolling updates
6. Health Checks

# Kubernetes

> OPEN SOURCE, CONTAINER ORCHESTRATION PLATFORM, FACILITATES DECLARATIVE MANAGEMENT, POSSESS A GROWING ECOSYSTEM, WIDELY AVAILABLE

# Kubernetes Cheatseet

|

1. ubectl apply = Apply a configuration to a resource.
2. kubectl config: get-clusters Displays clusters defined in the kubeconfig.
3. kubectl config: get-contexts Displays the current context.
4. kubectl create: Create a resource.
5. kubectl delete: Deletes resources.
6. kubectl describe: Shows details of a resource or group of resources.
7. kubectl expose: Expose a resource to the internet as a new Kubernetes service.
8. kubectl get: Displays resources.
9. kubectl get: pods Lists all the Pods in the namespace.
10. kubectl proxy: Creates a proxy server between a localhost and the Kubernetes API
    server.
11. kubectl rollout: Manage the rollout of a resource.
12. kubectl run: Creates and runs a particular image in a pod.
13. kubectl scale: Set a new size for a deployment.
14. kubectl set: Configure application resources.
15. kubectl version: Prints the client and server version information

# Glossary Kubernetes

1. Cluster= A deployment of Kubernetes.
2. Container Orchestration =Aids in the provisioning and deployment of containers
   to make this a more automated, unified, and smooth
   process. Container orchestration ensures that
   containers are redundant and available so that
   applications experience minimal downtime. It scales
   containers up and down to meet demand, and it load-
   balances requests across instances so that no one
   instance is overwhelmed. It handles the scheduling of
   containers to underlying infrastructure. Lastly,
   container orchestration tools can perform health checks
   to ensure that applications are running, and these
   tools can take necessary actions when checks fail.
3. Control Loop = A non-terminating loop that regulates the state of a
   system. A thermostat is an example of a control loop.
4. Declarative Management =A desired state that can be expressed (for example, the
   number of replicas of a specific application),and
   Kubernetes will actively work to ensure that the
   observed state matches the desired state.
5. Deployment = An object that provides updates for both Pods and
   ReplicaSets. Deployments run multiple replicas of an
   application by creating ReplicaSets and offering
   additional management capabilities on top of those
   ReplicaSets. In addition, deployments are suitable for
   stateless applications.
6. = Docker A popular container runtime that is responsible for
   downloading images and running containers. Rather than
   providing a single container runtime, Kubernetes
   implements a Container Runtime Interface that permits
   pluggability of the container runtime.
7. etcd = A highly available key value store that contains all
   the cluster data. When someone tells Kubernetes to
   deploy an application, that deployment configuration is
   stored in etcd. It is the source of truth for the state
   in a Kubernetes cluster, and the system works to bring
   the cluster state into line with what is stored in
   etcd.
8. Imperative Management = Defining steps and actions to get to a desired state.
9. Kubelet = This controller communicates with the Kubernetes API
   server to receive new and modified Pod specifications
   and ensure that Pods and their associated containers
   are running as desired. The kubelet also reports to the
   control plane on health and status.
10. = Kubernetes A portable, extensible, open-source platform for
    managing containerized workloads and services that
    facilitates both declarative configuration and
    automation.
11. Kubernetes Controller Manager = Runs all the controller processes that monitor the
    cluster state and ensure that the actual state of a
    cluster matches the desired state. The cloud controller
    manager runs controllers that interact with the
    underlying cloud providers. These controllers
    effectively link clusters into a cloud provider’s API.
12. Kubernetes Proxy = A network proxy that runs on each node in a cluster.
    This proxy maintains network rules that allow
    communication to Pods running on nodes—in other words,
    communication to workloads running on the cluster.
13. Label Selector = The core grouping primitive in Kubernetes. They
    identify a set of objects.
14. Labels = A key/value pair that can be attached to objects in
    order to identify those objects.
15. Namespace = Provides a way to make one cluster appear to be several
    distinct clusters. They provide an isolated workspace
    for the container. When a container is run, Docker
    creates a set of namespaces for that container. They
    provide a layer of isolation. Each aspect of a
    container runs in a separate namespace, and its access
    is limited to that namespace.
16. Node = The worker machine in a Kubernetes cluster. User
    applications are run on nodes. Nodes can be virtual or
    physical machines. Each node is managed by the control
    plane and is able to run Pods.
17. Persistence = Ensures that an object exists in the system, until the
    object is modified or removed.
18. Pod = Represents a process running in a cluster; it also
    represents a single instance of an application running
    in a cluster. Usually, a Pod wraps a single container.
    Although in some cases, a Pod can encapsulate multiple
    tightly coupled containers that share resources.
19. ReplicaSet = A group of identical Pods that are running. The object
    used to scale an application by running replicas of a
    Pod.
20. YAML = File Defines the object or objects that you want to create
