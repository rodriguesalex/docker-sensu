# Set the base image
FROM ubuntu:16.04

MAINTAINER Alex Rodrigues <rodrigues.alex@gmail.com>

# Install Redis from the distribution repository
RUN apt-get update
RUN apt-get -y install redis-server

# Enable Redis to start on system boot
RUN update-rc.d redis-server enable

# Start the Redis service
ENTRYPOINT ["/usr/bin/redis-server"]

# Expose default port
EXPOSE 6379