FROM golang:1.15-alpine

WORKDIR /go/src/app
ADD ./app /go/src/app

RUN apk update && \
    apk add --no-cache git && \
    go get github.com/labstack/echo/... && \
    go get github.com/pilu/fresh

EXPOSE 8080

CMD ["fresh"]