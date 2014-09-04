FROM aputs/golang

VOLUME /opt/bin

RUN go get -d github.com/coreos/rudder
RUN go build -o /opt/bin/rudder github.com/coreos/rudder
