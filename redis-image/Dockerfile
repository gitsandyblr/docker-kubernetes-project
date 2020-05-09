# Use an existing docker image as a base
FROM alpine

#Rebuilding with cache - it improves docker performance
RUN apk add --update gcc

# Download and install a dependency
RUN apk add --update redis

# Tell the image what to do when it starts as a container
CMD ["redis-server"]