## CONFIGURACAO DO AMBIENTE COM AS DEPENDENCIAS
FROM ubuntu:latest as enviroment

RUN apt update && apt install curl build-essential -y

## COMPILACAO DO CODIGO
FROM enviroment as builder

WORKDIR /src

COPY . /src

RUN g++ main.cpp -o main

CMD ["./main"]