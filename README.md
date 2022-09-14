# General

After starting application (see instructions below), navigate to `http://localhost/`.

MySQL admin tool at `http://localhost:8000/`.  To log in, use `mysql_db` as the server, `root` as the user, and `MYSQL_ROOT_PASSWORD` for the password.

# Dev Environment

To start local dev environment
```
docker compose -f docker-compose.dev.yml up --build
```

To delete all containers, volumes, and images.
```
docker rm $(docker ps -a -q)
docker volume rm $(docker volume ls -q)
docker image rm $(docker images -a -q)
```

# Prod Environment

To start environment in prod mode
```
docker compose up --build
```
