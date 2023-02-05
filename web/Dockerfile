FROM golang

WORKDIR /app
COPY . .
RUN CGO_ENABLED=0 go build dispatcher.go

FROM scratch
COPY --from=0 /app/dispatcher .

CMD ["./dispatcher"]
