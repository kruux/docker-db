# docker-db

A docker stack using postgres and a homegrown backup container.

Usage
```console
$ echo "yourOwnSecretPassword" > postgres_password.secret
$ chmod 700 postgres_password.secret
$ sudo chown root:root postgres_password.secret
$ sudo docker stack deploy -c docker-stack.yml db
```

##### Todo
* Add rotation to the backups
* Write a REST API in a new container.
