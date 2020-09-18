FROM node:12

RUN apt-get update && \
    apt-get update -yy && \
    apt-get install git -yy

RUN git clone https://github.com/h8a/productivity_prod.git

WORKDIR /productivity_prod

RUN npm install

EXPOSE 3000:3000

CMD [ "node", "index" ]