FROM golang:alpine
RUN apk --no-cache add gcc g++ make ca-certificates git
WORKDIR /go/src/

RUN ["go", "get", "github.com/githubnemo/CompileDaemon"]

ENTRYPOINT cd ./query-service && GO111MODULE=on CompileDaemon -build="go build" -command="./query-service"
