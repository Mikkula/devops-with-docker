```
root@debian-8gb-hel1-docker:~# docker run -p 80:80 devopsdockeruh/ports_exercise

> ports_exercise@1.0.0 start /usr/app
> node index.js

Listening on port 80, this means inside of the container. Use -p to map the port to a port of your local machine.
```
Output
```
root@debian-8gb-hel1-docker:~# curl http://localhost
Ports configured correctly!!
```
