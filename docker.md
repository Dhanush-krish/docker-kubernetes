
### Docker
* translator between human and kernel
* **docker -> dockerd -> containerd(runtime)** (to run containers)
* dockerd offers other features like volumes, logs, ux than containerd
* containers lasts only till the program you started with it lasts. It will stop immediately after the program exists.
* build context - Docker demon copies all the content in build context before building docker file.
  


### Docker File commands
#### build time Instructions
*  **FROM**      -> pulls base imange from repository
*  **RUN**       -> executes commands
*  **WORKDIR**   -> created directory and executes subsequent commands in that directory
*  **COPY**      -> src is build context dest is WORKDIR
*  **ADD**       -> src can be remote also extracts tar files
*  **ENV**       -> sets environment variables in container environment

#### launch time Instructions
*  **EXPOSE**    -> port at which app inside the container runs
*  **CMD**        -> used to start application commands in fg
*  **ENTRYPOINT** ->  used to execute application initialization scripts
*  **ENTRYPOINT executes first then CMD**

### Multi stage docker file
* creates image that contains application, runtime 
* splits the docker file into multiple images
* only the last image is published to registry
* It reduces the image size by eliminating unnecessary dependencies need for build and test step.

### Docker file - best Practices
* file name should start with capital letter **Dockerfile**
* Commands in dockerfile should be in uppercase
* each command in docker file creates a new layer
* combine multiple commands as one RUN commmand
* docker allows maximum **128 layer**
* always keep you build context light to reduce build time - don't keep docker file in root dir.
  
