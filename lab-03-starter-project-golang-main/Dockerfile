FROM golang

WORKDIR /app

COPY go.mod so.sum ./

RUN go mod download

COPY . .

RUN go build -o build/fizzbuzz

EXPOSE 8080

CMD ["./build/fizzbuzz", "serve"]