# mongo-node-8
Dockerfile - MongoDb with node 8

This image can be used as a base image for your projects. It contains mongo 3.4 and node 8.

The default WORKDIR is `/usr/src/app`

## Example

```docker
FROM concreteplatform/mongo-node-8

ENV NODE_ENV=test

# Set environment path for mongodb
ENV MONGO_URL=mongodb://localhost/concrete-one-test
ENV DB_MONGO=localhost/concrete-one-test
CMD ["bin/run-tests-in-docker.sh"]
```