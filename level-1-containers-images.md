Level 1: Containers & Images
====

- Linux containers
  - A way to create isolated environments that can run code while sharing a single operating system.
  - Completely isolated from each other.

- Docker
  - A tool to manage Linux containers.

- Ways to use Docker
  - Developers
    - Create contained, controlled dev environment
      - Focus of this course
    - Share identical dev environment across team
    - Bug reporting
  - IT ops
    - Testing
    - Deployment

- Image
  - A blueprint for creating a container
  - Pre-built images available in Docker Store (and Docker Hub)

- Running a container
  - `docker container run -p <host-port>:<container-port> <image>:<version>`
  - `-p`: publish ports
  - `--detach`: make the container run in the background

- Accessing a container
  - `docker container ls`
  - `docker container exec <container-id-or-name> <command>`

- Attaching a shell to a container
  - `docker container exec -it <container-id-or-name> /bin/bash`
