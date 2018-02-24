Level 3: Volumes
====

# Get data into container
- Copy file into container from command line
  - `docker container cp <local-file> <container-id>:<container-location>`

- Copy file into image with instructions in a Dockerfile
  - `COPY <local-file> <container-location>`

# Problem
- Containers don't persist data

# Solution
- Data volumes: expose files on host machine to the container
  - Create a link between host and conatiner
  - docker run -v <local-location>:<container-location> <image>:<version>
