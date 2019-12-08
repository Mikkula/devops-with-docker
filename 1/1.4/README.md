```
root@debian-8gb-hel1-docker:~# docker run -d devopsdockeruh/exec_bash_exercise
bf0a4bc7580f0ad94433e0e034f5e52abac5203f3a50951b1ff1fbffc0b961bb
root@debian-8gb-hel1-docker:~# docker ps -a
CONTAINER ID        IMAGE                               COMMAND             CREATED             STATUS                     PORTS               NAMES
bf0a4bc7580f        devopsdockeruh/exec_bash_exercise   "node index"        3 seconds ago       Up 2 seconds                                   unruffled_fermi
root@debian-8gb-hel1-docker:~# docker exec -it unruffled_fermi bash
root@bf0a4bc7580f:/usr/app# tail -f ./logs.txt
Thu, 17 Oct 2019 17:38:25 GMT
Thu, 17 Oct 2019 17:38:28 GMT
Thu, 17 Oct 2019 17:38:31 GMT
Thu, 17 Oct 2019 17:38:34 GMT
Secret message is:
"Docker is easy"
Thu, 17 Oct 2019 17:38:40 GMT
Thu, 17 Oct 2019 17:38:43 GMT
Thu, 17 Oct 2019 17:38:46 GMT
Thu, 17 Oct 2019 17:38:49 GMT
Secret message is:
"Docker is easy"
```
