## 1.12

## Doing it with new Dockerfiles/containers
Doing the exercise exactly as guided here (setting the env vars in Dockerfile).
```
docker build -t frontend -f Dockerfile.frontend .
docker build -t backend -f Dockerfile.backend .
docker run -d -p 5000:5000 frontend
docker run -d -p 8000:8000 backend
```

## Doing it with the 1.10 and 1.11 containers (IMO better way)

I would really do the exercise using the old containers from previous exercises. This way the Dockerfile/container stays as generic as possible, and it can be configured from "outside" using the -e flag.

For this exercise to work properly we have to change the 1.10 container to build the frontend on runtime, not on Docker image build :(.

Starting frontend container from 1.10:
```
docker run -p 5000:5000 -e API_URL="http://localhost:8000" ten 
```

Starting backend container from 1.11:
```
docker run -p 8000:8000 -e FRONT_URL="http://localhost:5000" eleven
```
