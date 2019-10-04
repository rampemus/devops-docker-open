FROM ubuntu:16.04

RUN apt-get update && apt-get install -y wget

WORKDIR /mydir
RUN touch hello.txt
COPY local.txt .
RUN wget http://example.com/index.html
CMD ["/bin/bash"]
