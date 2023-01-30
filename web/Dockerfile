FROM golang

COPY . .
RUN go build dispatcher.go
CMD exec ./dispatcher
