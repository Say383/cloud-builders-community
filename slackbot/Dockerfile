FROM gcr.io/cloud-builders/go AS build-env

WORKDIR /app
COPY . .

RUN go get -v
RUN go build main.go

FROM alpine:3.18.3

RUN apk add --no-cache ca-certificates

COPY --from=build-env /app/main /app/main

ENTRYPOINT [ "/app/main" ]
