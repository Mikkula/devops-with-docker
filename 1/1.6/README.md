```
root@debian-8gb-hel1-docker:~/temp# docker build -t docker-clock .
Sending build context to Docker daemon  2.048kB
Step 1/2 : FROM devopsdockeruh/overwrite_cmd_exercise
latest: Pulling from devopsdockeruh/overwrite_cmd_exercise
092586df9206: Pull complete
ef599477fae0: Pull complete
4530c6472b5d: Pull complete
d34d61487075: Pull complete
87fc2710b63f: Pull complete
e83c771c5387: Pull complete
fef6195892ae: Pull complete
70e1a68db517: Pull complete
c2599bbef3cb: Pull complete
c5a7dd6f6ae1: Pull complete
446220381e79: Pull complete
27d5280e809c: Pull complete
Digest: sha256:02e38f4285d5cfaff5ed57ae67a8d99e041027da8f5c972329b46e2b7a47b7d2
Status: Downloaded newer image for devopsdockeruh/overwrite_cmd_exercise:latest
 ---> 3d2b622b1849
Step 2/2 : CMD ["-c", "0"]
 ---> Running in 5a9f8fe9312b
Removing intermediate container 5a9f8fe9312b
 ---> 47d362cea97f
Successfully built 47d362cea97f
Successfully tagged docker-clock:latest
root@debian-8gb-hel1-docker:~/temp# docker run docker-clock
1
2
3
4
5
6
7
8
9
10
```
