```
root@debian-8gb-hel1-docker:~# touch logs.txt
root@debian-8gb-hel1-docker:~# docker run -d -v $(pwd)/logs.txt:/usr/app/logs.txt devopsdockeruh/first_volume_exercise
64e8fe44d12a6d88dc9e21d2f45f2f35dd93e80359ef908943ce574a8c9823e2
root@debian-8gb-hel1-docker:~# tail -f logs.txt
Thu, 17 Oct 2019 19:22:03 GMT
Thu, 17 Oct 2019 19:22:06 GMT
Thu, 17 Oct 2019 19:22:09 GMT
Thu, 17 Oct 2019 19:22:12 GMT
Secret message is:
"Volume bind mount is easy"
^C
root@debian-8gb-hel1-docker:~#
```
