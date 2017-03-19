This Dockerfile produces an image with the TexLive package installed.

You can use this to compile your Latex Documents.

##Usage

You can build the Docker image yourself using the following commands:

    git clone 
    cd texlive-docker
    docker build -t tex .

After that, you can start a TexLive Docker container. The Latex source files should be mounted to /doc and the output is also written to that directory. Please provide a Makefile in /doc to tell the container what to do. An example can be found in the /exaple directory

    docker run -v "/example":"/doc" tex


