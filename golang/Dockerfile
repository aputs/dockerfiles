FROM debian:stable
MAINTAINER Allan Ralph Hutalla <ahutalla@gmail.com>

RUN apt-get update -q
RUN DEBIAN_FRONTEND=noninteractive apt-get install -qy build-essential curl git mercurial bzr ca-certificates
RUN curl -s https://storage.googleapis.com/golang/go1.3.1.src.tar.gz | tar -v -C /usr/local -xz
RUN cd /usr/local/go/src && ./make.bash --no-clean 2>&1
ENV PATH /usr/local/go/bin:$PATH
ENV GOPATH /golang
