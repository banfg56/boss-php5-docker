FROM centos:7

RUN yum update -y && \
    yum install -y epel-release

RUN yum install -y nginx

COPY ./conf/nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./conf/nginx/crm3.conf /etc/nginx/conf.d/crm3.conf

RUN yum clean all

CMD nginx
