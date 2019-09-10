FROM centos:latest
WORKDIR /home
COPY . ${WORKDIR}
RUN yum update && yum install pip && pip install flask
EXPOSE 5000
ENTRYPOINT ["python","index.py"]