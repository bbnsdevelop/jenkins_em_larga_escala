FROM jenkins/jenkins:lts
USER root
COPY apt.conf /etc/apt/apt.conf
RUN apt-get update && apt-get install -y make git openjdk-8-jdk
VOLUME /usr/share/jenkins/:/usr/share/jenkins/
USER jenkins
ENV JAVA_HOME /usr/lib/jvm/java-8-openjdk-amd64