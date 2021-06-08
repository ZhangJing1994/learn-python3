FROM golang:alpine3.13
WORKDIR  /go/src
ENV GO111MODULE=on
ENV GOPROXY="https://goproxy.io"
ADD . /go/src
# RUN  chomd 777 /go/src
EXPOSE 8088
RUN cd /go/src && go build -o main 
CMD ["/go/src/main"]
