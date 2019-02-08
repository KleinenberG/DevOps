FROM ubuntu:trusty
WORKDIR /opt/webapp
ADD webapp/ /opt/webapp/
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y -q python-all python-pip
RUN pip install -qr requirements.txt
EXPOSE 5000
CMD ["python", "app.py"]
