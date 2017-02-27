# docker-ubuntu-ssh

Docker image with sshd server for local development of the my ansible scripts.

Run container:
```
$ docker pull rafaelrsantos/ubuntu-ssh
$ docker run -d -p 22000:22 --name ssh-test rafaelrsantos/ubuntu-ssh
$ docker port ssh-test 22
...

0.0.0.0:22000
```

Connect to the custom ssh port 22000:
```
# The password is "toor".
$ ssh root@localhost -p 22000
...
```
