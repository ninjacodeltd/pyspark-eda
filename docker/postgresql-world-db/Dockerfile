# Init Example Database World on PostgreSQL
FROM postgres:16.1-bullseye

ENV POSTGRES_USER world
ENV POSTGRES_PASSWORD world123
ENV POSTGRES_DB world-db

ADD data/*.sql /docker-entrypoint-initdb.d/
ADD data/*.csv /docker-entrypoint-initdb.d/
