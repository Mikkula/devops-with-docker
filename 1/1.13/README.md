## 1.13

The image could be made smaller by using multi-stage Docker build (we don't need jdk or build dependencies at runtime)

```
docker build -t thirt .
docker run -p 8080:8080 thirt
```
