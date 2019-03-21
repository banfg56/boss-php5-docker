FROM centos:7

RUN yum update -y && \
    yum install -y epel-release

RUN yum install -y nginx

COPY ./conf/nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./conf/nginx/bizz2.conf /etc/nginx/conf.d/bizz2.conf

RUN yum clean all

CMD nginx
