FROM mongo:4.2.2-bionic

ENV MONGO_INITDB_ROOT_USERNAME admin
ENV MONGO_INITDB_ROOT_PASSWORD secret
ENV MONGO_INITDB_DATABASE online

COPY mongo-init.js /docker-entrypoint-initdb.d/
EXPOSE 27017
VOLUME /data/db

#docker run --name some-mongo -p 27017:27017 -d mongo:4.2.2-bionic