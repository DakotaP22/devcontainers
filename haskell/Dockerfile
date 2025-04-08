# Use the official Ubuntu image as the base image
FROM ubuntu:latest

# Set the environment variable for non-interactive installation
ENV DEBIAN_FRONTEND=noninteractive

# Update the package list and install necessary tools
RUN apt-get update && \
    apt-get install -y \
    curl 


RUN curl -sSL https://get.haskellstack.org/ | sh


# Set the default command to run when the container starts
CMD ["/bin/bash"]