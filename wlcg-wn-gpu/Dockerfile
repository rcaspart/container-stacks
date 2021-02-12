FROM matterminers/wlcg-wn:latest
MAINTAINER Rene Caspart <rene.caspart@kit.edu>

COPY files/nvidia-machine-learning.repo /etc/yum.repos.d/
COPY files/nvidia-cuda.repo /etc/yum.repos.d/

RUN yum update -y && \
    yum install -y kernel-devel kernel-header
RUN yum install -y nvidia-driver-latest-dkms cuda-drivers && \
    yum clean -y all
