FROM ubuntu:18.04

RUN apt-get update && apt install -y nmap

COPY ./tests.sh /tmp/

WORKDIR /tmp 

# safe to pass env vars here because this image is not hosted on docker hub
ENTRYPOINT ["sh", "-c", "/tmp/tests.sh"]