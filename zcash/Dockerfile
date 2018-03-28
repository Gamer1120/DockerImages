FROM python:2.7-slim

ADD . /zcash

RUN mkdir .zcash ; apt-get update && apt-get install libgomp1 wget -y

RUN ./zcash/go-ipfs/install.sh ; ./zcash/zcash/bin/zcash-fetch-params ; 

#Due to technical limitations, please copy zcash.conf in this directory
#to the /zcash directory on the host
#ADD zcash.conf /root/.zcash/zcash.conf

CMD ./zcash/zcash/bin/zcashd 
