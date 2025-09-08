FROM ubuntu:latest
RUN apt-get update && \
apt-get upgrade -y && \
apt-get install -y python3 && \
apt-get install -y python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask
RUN pip3 flask-cors
WORKDIR /app
COPY ./api.py /app/.api.py
CMD ["python3", "api.py"]
