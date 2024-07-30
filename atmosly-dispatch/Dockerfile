FROM golang:1.21

WORKDIR /go/src/app

COPY atmosly-dispatch/*.go .

RUN go mod init dispatch && go get
RUN go install

CMD dispatch
