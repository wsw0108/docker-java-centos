FROM centos:6

MAINTAINER wsw0108 <wsw0108@foxmail.com>


RUN yum update -y && \
yum install -y wget && \
wget https://mirror.its.sfu.ca/mirror/CentOS-Third-Party/NSG/common/x86_64/jre-7u80-linux-x64.rpm && \
yum localinstall -y /jre-7u80-linux-x64.rpm && \
rm -f /jre-7u80-linux-x64.rpm && \
rm -rf /var/cache/yum

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /data
VOLUME /data

# Define default command.
CMD ["bash"]

