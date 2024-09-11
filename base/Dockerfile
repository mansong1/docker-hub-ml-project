FROM python:3.12.5

RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential

COPY /requirements.txt /tmp/
RUN cd /tmp && \
    pip install --no-cache-dir -r requirements.txt

# copy python scripts
COPY ./src /src
