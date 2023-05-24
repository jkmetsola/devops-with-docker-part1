FROM golang:1.16

COPY ./material-applications/example-backend /example-backend

WORKDIR /example-backend

ENV PORT=8080
ENV REQUEST_ORIGIN=https://127.0.0.1

RUN pwd
RUN go build
RUN go test ./...
CMD ./server



EXPOSE 8080