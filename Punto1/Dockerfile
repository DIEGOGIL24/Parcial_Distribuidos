FROM alpine:3.20

RUN apk add --no-cache curl

WORKDIR /app
COPY mensaje.txt /app

EXPOSE 7015

CMD ["cat","mensaje.txt"]
