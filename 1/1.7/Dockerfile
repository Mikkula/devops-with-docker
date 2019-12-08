FROM ubuntu:18.04
RUN apt-get update && apt-get install -y curl

COPY script.sh ./
RUN chmod +x script.sh

CMD ["bash", "script.sh"]
