FROM centos:latest
WORKDIR /home
COPY . ${WORKDIR}
RUN yum update -y &&  yum -y install epel-release && yum install python-pip && pip install flask
EXPOSE 5000
ENTRYPOINT ["python","index.py"]
