## 1.17

Python 3 programming environment. Installs python3 and pip3.

```
docker build -t py .
# Runs bash
docker run -it --rm -v $(pwd):/develop:/develop py 
docker run -it --rm -v $(pwd):/develop:/develop py python3 
