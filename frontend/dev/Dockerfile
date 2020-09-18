FROM node:12

RUN apt-get update && \
    apt-get update -yy && \
    apt-get install git -yy

RUN git clone https://github.com/h8a/productivity.git

WORKDIR /productivity

RUN npm install && \
    npm install -g @angular/cli

EXPOSE 4200:4200

CMD [ "ng", "serve", "--host=0.0.0.0", "--disable-host-check" ]