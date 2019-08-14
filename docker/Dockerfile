FROM ubuntu:16.04

RUN \
apt update -y\
&& apt install -y curl \
&& curl -sL https://deb.nodesource.com/setup_8.x | bash -

RUN \
apt-get install -y nodejs\
&& apt-get install npm \
&& npm install npm -g 

RUN cd /root && apt install git\
&& git clone https://github.com/yutiansut/adminmongo \
&& cd adminmongo && npm install

EXPOSE 12345
CMD ["cd /root/adminmongo && npm start"]

