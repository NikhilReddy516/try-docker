Level 2: Dockerfiles
====

- Dockerfile
  - A list of instructions that will run and result in a new image that   can be used to make a container.
  - Filename: `Dockerfile`


- Create Dockerfile

  ```
  FROM <base-image-name>:<version>

  EXPOSE <container-port>

  RUN <command>

  LABEL key="value"
  ```

- Build image from Dockerfile
  - Build: `docker image build --tag <tag-name>:<version> <dockerfile-location>`
  - Browse: `docker image ls`
