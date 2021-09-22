# docker-oracledb21c-xe
Temporary Docker files and scripts for [Oracle Database 21c Express Edition](https://oracle.com/xe).

The scripts are modified versions of Oracle's official Dockerfiles and scripts for Oracle Database 18c Express Edition that you can find [here](https://github.com/oracle/docker-images/tree/main/OracleDatabase/SingleInstance/dockerfiles/18.4.0).

This repository will be archived as soon as Oracle releases the updated files for this version of the database.

To build the Docker image, run the command:

```bash
docker build -t oracle/database:21.3.0-xe .
```

To run a container based on this image, run the command:

```bash
CONTAINER_NAME=myxedb && \
docker run -d -p 1521:1521 --name $CONTAINER_NAME oracle/database:21.3.0-xe
```

Some of the Docker run options listed [here](https://github.com/oracle/docker-images/tree/main/OracleDatabase/SingleInstance) could be used too.