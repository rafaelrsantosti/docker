# docker-ubuntu-ssh

Docker image with sshd server for local development of the my ansible scripts.

Run container:
```
$ docker pull rafaelrsantos/ubuntu-ssh
$ docker run -d -P --name ssh-test rafaelrsantos/ubuntu-ssh
$ docker port ssh-test 22
...

0.0.0.0:32769
```

Connect to the custom ssh port (example: 32769):
```
# The password is "toor".
$ ssh root@localhost -p 32769
...
```
