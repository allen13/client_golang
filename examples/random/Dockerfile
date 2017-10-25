FROM golang:1.9.0
WORKDIR /go/src/github.com/prometheus/client_golang/examples/random
COPY . .
RUN go get -d
RUN CGO_ENABLED=0 GOOS=linux go build -a -tags netgo -ldflags '-w'
CMD ["/random"]
