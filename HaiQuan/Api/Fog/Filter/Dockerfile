FROM python:3.5-slim

MAINTAINER HaiQuan "haiquan5396@gmail.com"

ENV BROKER_FOG localhost

COPY ./requirements.txt /app/requirements.txt

WORKDIR /app

RUN pip3 install -r requirements.txt

COPY ./Filter.py /app

CMD python3 Filter.py ${BROKER_FOG}

#docker build -t haiquan5396/filter:1.2 -f .
#docker run -it --name filter-test -e "BROKER_CLOUD=192.168.60.248" haiquan5396/filter:1.2