FROM quay.io/centosci/cico-workspace:latest

MAINTAINER Alfredo Moralejo <amoralej@redhat.com>

USER 0

RUN rm -f /etc/yum.repos.d/infrastructure.repo
RUN yum install -y python3 python3-pip && yum clean all
RUN curl https://bootstrap.pypa.io/pip/2.7/get-pip.py --output get-pip.py && python2 ./get-pip.py
RUN pip install tox

USER 1001
