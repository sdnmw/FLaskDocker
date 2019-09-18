FROM centos

MAINTAINER "mw"

COPY flask_demo.py /home/

COPY start_flask.sh /usr/local/

RUN yum -y install epel-release && \
    
    yum -y install python-pip && \
    
    yum clean all && \
    
    pip install flask && \
    
    chmod +x /usr/local/start_flask.sh

EXPOSE 80

#start flask

ENTRYPOINT /usr/local/start_flask.sh
