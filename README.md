## Java with CentOS 6

This is docker images of CentOS 6 with different versions of java
> Fork from https://github.com/nimmis/docker-java-centos

### Loading different versions of java

The different version is determined with the TAG

The available version are

* latest                 - currently Oracle Java version 9 JRE
* openjdk-7-jdk          - OpenJDK Java version 7 JDK
* openjdk-7-jre          - OpenJDK Java version 7 JRE
* openjdk-8-jdk          - OpenJDK Java version 8 JDK
* openjdk-8-jre          - OpenJDK Java version 8 JRE
* openjdk-8-jre-headless - OpenJDK Java version 8 JRE headless
* oracle-7-jre           - Oracle Java version 7 JRE
* oracle-7-jdk           - Oracle Java version 7 JDK
* oracle-8-jre           - Oracle Java version 8 JRE
* oracle-8-jdk           - Oracle Java version 8 JDK
* oracle-9-jre           - Oracle Java version 9 JRE
* oracle-9-jdk           - Oracle Java version 9 JDK

Example to run a container with OpenJDK version 7 JDK

  `docker run -ti wsw0108/java-centos6:openjdk-7-jdk`
