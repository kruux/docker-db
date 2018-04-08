# docker-db

A docker stack using postgres and a homegrown backup container.
Only tested with docker 18.03

Usage
```console
$ echo "yourOwnSecretPassword" > postgres_password.secret
$ chmod 600 postgres_password.secret
$ sudo chown root:root postgres_password.secret
$ sudo docker stack deploy -c docker-stack.yml db
```

##### Todo
* Add rotation to the backups
* Write a REST API in a new container.
