FROM golang:1.13.8
RUN mkdir -p /go/src/MyApp
ADD . /go/src/MyApp
 
RUN go get github.com/revel/revel
RUN go get github.com/revel/cmd/revel
 
WORKDIR /go
ENTRYPOINT revel run -a MyApp
EXPOSE 9000
