FROM ubuntu:latest
RUN apt-get update
RUN apt-get upgrade -y
RUN apt install python3 -y
RUN apt install python3-pip -y
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask

WORKDIR /app
COPY ./api.py /app/api.py

EXPOSE 5252

CMD ["python3", "api.py" ]