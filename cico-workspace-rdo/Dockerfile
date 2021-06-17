FROM quay.io/centosci/cico-workspace:latest

MAINTAINER Alfredo Moralejo <amoralej@redhat.com>

USER 0

RUN rm -f /etc/yum.repos.d/infrastructure.repo
RUN yum install -y python3 python3-pip && yum clean all

USER 1001
