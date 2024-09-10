# Specify a base image : Use an existing docker image as a base
FROM alpine

# Run some commands to install additional programs : Download and install a dependency
RUN apk add --update redis

# Specify a command to run on container startup : Tell the image what to do when it starts as a container
CMD ["redis-server"]

# docker build .
# docker run #(hash)