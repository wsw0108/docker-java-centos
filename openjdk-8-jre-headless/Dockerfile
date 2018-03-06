FROM centos:6

MAINTAINER wsw0108 <wsw0108@foxmail.com>

RUN yum update -y && \
yum install -y wget && \
yum install -y java-1.8.0-openjdk-headless && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /data
VOLUME /data

# Define default command.
CMD ["bash"]

