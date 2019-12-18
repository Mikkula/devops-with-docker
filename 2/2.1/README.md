## 2.1

We have to ensure that the logs.txt file exists before starting so Docker doesn't create directory instead.

```
# touch logs.txt
# docker-compose up
Starting 21_first_volume_exercise_1 ... done
Attaching to 21_first_volume_exercise_1
first_volume_exercise_1  | (node:1) ExperimentalWarning: The fs.promises API is experimental
first_volume_exercise_1  | Wrote to file /usr/app/logs.txt
first_volume_exercise_1  | Wrote to file /usr/app/logs.txt
first_volume_exercise_1  | Wrote to file /usr/app/logs.txt
first_volume_exercise_1  | Wrote to file /usr/app/logs.txt
^CGracefully stopping... (press Ctrl+C again to force)
Stopping 21_first_volume_exercise_1 ... done
# cat logs.txt 
Wed, 18 Dec 2019 18:49:50 GMT
Wed, 18 Dec 2019 18:49:53 GMT
Wed, 18 Dec 2019 18:49:56 GMT
Wed, 18 Dec 2019 18:49:59 GMT
```
