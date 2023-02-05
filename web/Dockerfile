FROM golang:alpine

WORKDIR /app
COPY . .
RUN go build dispatcher.go

FROM alpine
COPY --from=0 /app/dispatcher .

CMD ["./dispatcher"]
