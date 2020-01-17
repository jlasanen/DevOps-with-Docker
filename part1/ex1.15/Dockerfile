# exercise 1.15
FROM ubuntu:16.04


# install curl
RUN apt-get update && apt-get install -y curl

# install git
RUN apt-get install -y git

# get OpaaliAPI scripts
RUN git clone https://github.com/jlasanen/OpaaliAPI.git
WORKDIR /OpaaliAPI/scripts
RUN chmod ugo+x *.sh

RUN echo "\nrun as interactive shell to send text messages\n"

CMD /bin/bash

