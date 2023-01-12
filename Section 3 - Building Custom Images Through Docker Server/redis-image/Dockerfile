# Use an existing docker image as a base
FROM alpine

# Download and install a dependency
RUN apk add --update redis

# Tell the image what to do when it starts as a container
CMD ["redis-server"]

# Tagging an image with docker {DockerID} / {ProjectName} / {Version}
# But technically the repo is the project name then the version is the actual tag for the image.