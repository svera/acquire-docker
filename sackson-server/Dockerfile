FROM golang:1.7-alpine
RUN apk add --no-cache git
RUN go get github.com/svera/sackson-server
ADD ./config /config
WORKDIR /config
CMD sackson-server
