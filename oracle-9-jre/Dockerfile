FROM centos:6

MAINTAINER wsw0108 <wsw0108@foxmail.com>

ENV JAVA_VERSION_FULL=9.0.4 \
    JAVA_VERSION_BUILD=11 \
    JAVA_URL_HASH=c2514751926b4512b076cc82f959763f

RUN yum update -y && \
yum install -y wget && \
wget --no-cookies --no-check-certificate \
  --header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2F; oraclelicense=accept-securebackup-cookie" \
  "http://download.oracle.com/otn-pub/java/jdk/${JAVA_VERSION_FULL}+${JAVA_VERSION_BUILD}/${JAVA_URL_HASH}/jre-${JAVA_VERSION_FULL}_linux-x64_bin.rpm" && \
yum localinstall -y jre-${JAVA_VERSION_FULL}_linux-x64_bin.rpm && \
rm -f jre-${JAVA_VERSION_FULL}_linux-x64_bin.rpm && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /data
VOLUME /data

# Define default command.
CMD ["bash"]

