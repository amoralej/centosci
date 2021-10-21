FROM quay.io/centosci/cico-workspace:latest

MAINTAINER Alfredo Moralejo <amoralej@redhat.com>

USER 0

ENV LANG en_US.UTF-8
ENV LC_ALL en_US.UTF-8
RUN rm -f /etc/yum.repos.d/infrastructure.repo
RUN yum install -y python3 python3-pip sudo  && yum clean all
RUN yum update -y && yum clean all
RUN curl https://bootstrap.pypa.io/pip/2.7/get-pip.py --output get-pip.py && python2 ./get-pip.py
RUN pip install tox
RUN pip-3 install virtualenv

USER 1001
