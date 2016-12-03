FROM python:3.5
RUN apt-get update
RUN apt-get -y upgrade
ADD . /home
RUN pip install -r /home/requirements.txt
WORKDIR /home/api

# Client
EXPOSE 80
ENTRYPOINT ["/home/api.py"]
