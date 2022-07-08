FROM ubuntu:latest
RUN apt-get -y update
RUN apt-get install openjdk-8-jdk -y
RUN mkdir /usr/local/tomcat
WORKDIR /usr/local/tomcat/
ADD  https://dlcdn.apache.org/tomcat/tomcat-10/v10.0.22/bin/apache-tomcat-10.0.22.tar.gz .
RUN tar xvfz apache-tomcat-10.0.22.tar.gz
EXPOSE 8080
CMD  ["/usr/local/tomcat/apache-tomcat-10.0.22/bin/catalina.sh","run"]
