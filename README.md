# docker-r-s

Docker container to run R scripts

### Build this image

`docker build -t vladdsm/docker-r-s .`

### Run the container

`docker run -it --rm -v [LOCAL_FOLDER]:/03_output vladdsm/docker-r-s`

### Details

Dockerfile will provision copy code and needed data to the container image. Once container  will run an R script will be executed. Output of the script will be placed into the folder 03_output. This folder is mapped to the LOCAL_FOLDER hence the results will also be available on the local machine.