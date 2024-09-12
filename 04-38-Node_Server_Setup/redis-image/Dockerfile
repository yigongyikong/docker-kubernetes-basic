
# Specify a base image : Use an existing docker image as a base
FROM alpine

# Run some commands to install additional programs : Download and install a dependency
RUN apk add --update redis
RUN apk add --update gcc

# Specify a command to run on container startup : Tell the image what to do when it starts as a container
CMD ["redis-server"]

# 각 단계별 이미지가 cache에 저장되고, build를 다시하면 cache에 저장된 이미지를 재사용한다.
# 만약 각 단계별 순서가 변한다면, 이미지는 다시 만들어진다.