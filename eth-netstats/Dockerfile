FROM node:16-alpine

RUN apk add --no-cache git bash perl

RUN git clone https://github.com/cubedro/eth-netstats.git /eth-netstats

WORKDIR /eth-netstats

RUN npm install
RUN npm install -g grunt-cli@1.2.0 --unsafe-perm
RUN grunt

EXPOSE 3000

CMD ["npm", "start"]

