FROM python:2.7-slim

RUN apt-get update && apt-get install -y wget
ADD . /bitcoin
CMD ./bitcoin/bitcoin-0.16.0/bin/bitcoind 
