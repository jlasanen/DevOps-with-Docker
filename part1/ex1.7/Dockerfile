FROM ubuntu:16.04

RUN apt-get update && apt-get install -y curl
COPY myscript.sh .
CMD ["/bin/bash", "-c", "./myscript.sh"]
