FROM golang:1.16-alpine
RUN apk add bash ca-certificates git gcc g++ libc-dev

RUN mkdir /app 
ADD . /app/ 
WORKDIR /app 
RUN go mod download
RUN go build -v
RUN ls
CMD ["/app/RealTimeChat"]