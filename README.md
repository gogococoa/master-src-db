# Database setup

this project we use postgres run with docker

## Option 1: docker run

-   create container
-   --name [name]
-   -e [env]
-   -p [local port]:[docker port] port mapping
-   -d detach run container in background and print container ID
-   image to use
-   docker run --name [container's name] -e [env] -p [L port]:[D port] -d [image]

```
docker run --name master-src-postgres -e POSTGRES_PASSWORD=[YOUR PASSWORD] POSTGRES_DB=master-src-db -p 5432:5432 -d postgres
```

## Option 2: docker-compose.yml

```
docker-compose up -d
```
