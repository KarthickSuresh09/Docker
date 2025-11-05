Tasks To Be Performed:
1. Pull Ubuntu container
   FROM golang:1.19 AS builder
WORKDIR /app
COPY . .
RUN go build -o myapp

FROM alpine:3.16
COPY --from=builder /app/myapp /myapp
CMD ["/myapp"]
3. Run this container and map port 80 on the local
4. Install Apache2 on this container
5. Check if you are able to access the Apache page on your browser
