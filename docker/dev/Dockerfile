FROM golang:alpine
RUN apk --no-cache add gcc g++ make ca-certificates git
WORKDIR /go/src/

ENV PORT=8080

RUN ["go", "get", "github.com/codegangsta/gin"]

ENV GO111MODULE=on
