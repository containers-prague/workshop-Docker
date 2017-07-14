See app_v{1..3} from https://github.com/tomkukral/kuberentes-examples for some handy demos


---
#### Linux Namespaces

Provide resource isolation by "hiding them"

.center[
Namespace  | Purpose
-----------|------------
mnt        | Mount points
pid        | Provide independent process IDs
net        | Networking stack
icp        | Inter-process communication
uts        | Provide different hostnames
uid        | Privilege isolation and user identification
cgroup     | Prevent leaking control-group
]

---

### Funny numbers
[Survey: state of container usage](https://clusterhq.com/assets/pdfs/state-of-container-usage-june-2016.pdf)

.quote[79% of respondents said that their organizations run container technologies, with 76% of them in production environments]

---
### Important `docker run` options

  * `--attach`
  * `--cpuset-cpus`
  * `--detach`
  * `--device`
  * `--entrypoint`
  * `--env`
  * `--expose`
  * `--interactive (-i)`
  * `--link (-l)`
  * `--memory (-m)`
  * `--name`
  * `--net`
  * `--privileged`
  * `--restart`
  * `--rm`
  * `--tty (-t)`
  * `--volume`
  * `--volumes_from`
---
.quote[How to change parameters of started container?]
---
.quote[What is the difference between image and container?]
---

#### Docker commands:

* `attach`: Attach local standard input, output, and error streams to a running container
* `build`: Build an image from a Dockerfile
* `commit`: Create a new image from a container's changes
* `cp`: Copy files/folders between a container and the local filesystem
* `create`: Create a new container (don't start)
* `diff`: Inspect changes to files or directories on a container's filesystem
* `events`: Get real time events from the server
* `exec`: Run a command in a running container
* `export`: Export a container's filesystem as a tar archive
* `history`: Show the history of an image
* `images`: List images
---
* `import`: Import the contents from a tarball to create a filesystem image
* `info`: Display system-wide information
* `inspect`: Return low-level information on Docker objects
* `kill`: Kill one or more running containers
* `load`: Load an image from a tar archive or STDIN
* `login`: Log in to a Docker registry
* `logout`: Log out from a Docker registry
* `logs`: Fetch the logs of a container
* `pause`: Pause all processes within one or more containers
* `port`: List port mappings or a specific mapping for the container
* `ps`: List containers
* `pull`: Pull an image or a repository from a registry
* `push`: Push an image or a repository to a registry
* `rename`: Rename a container
* `restart`: Restart one or more containers
---
* `rm`: Remove one or more containers
* `rmi`: Remove one or more images
* `run`: Run a command in a new container
* `save`: Save one or more images to a tar archive (streamed to STDOUT by default)
* `search`: Search the Docker Hub for images
* `start`: Start one or more stopped containers
* `stats`: Display a live stream of container(s) resource usage statistics
* `stop`: Stop one or more running containers
* `tag`: Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
* `top`: Display the running processes of a container
* `unpause`: Unpause all processes within one or more containers
* `update`: Update configuration of one or more containers
* `version`: Show the Docker version information
* `wait`: Block until one or more containers stop, then print their exit codes




---
#### Important Dockerfile commands

* `FROM image` sets base image
* `LABEL key value` add labels to the image
* `ENV key value` set environment variable
* `RUN` executes commands in image
  * shell form: `RUN command`
  * exec form: `RUN ["executeable", "param1", "param2"]`
* `WORKDIR dir` set current working directory
* `ADD src dest` copies new files
* `CMD cmd` default command to be executed in container
* `EXPOSE port` inform about open ports
* `VOLUME volume` create mount point with volume
* `ENTRYPOINT` configure executable for container


