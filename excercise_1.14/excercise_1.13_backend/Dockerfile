FROM golang:1.16

COPY ./material-applications/example-backend /example-backend

WORKDIR /example-backend

ENV PORT=8080
ENV REQUEST_ORIGIN=http://localhost:5000
ENV REACT_APP_BACKEND_URL=http://localhost:8080

RUN pwd
RUN go build
RUN go test ./...
CMD ./server



EXPOSE 8080