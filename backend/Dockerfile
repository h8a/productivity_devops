FROM ubuntu

RUN apt-get update && \
    apt-get upgrade -yy && \
    apt-get install -yy git && \
    apt-get install -yy python3-pip && \
    pip3 install pipenv

RUN git clone https://github.com/h8a/productivity_api.git

WORKDIR /productivity_api

RUN pipenv lock -r > requirements.txt && \
    pip3 install -r requirements.txt

CMD [ "python3", "src/main.py" ]
