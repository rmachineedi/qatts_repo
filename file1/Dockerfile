FROM ubuntu:latest
RUN apt-get -y update
RUN mkdir /usr/local/tomcat/
WORKDIR /usr/local/tomcat/
RUN apt-get install openjdk-8-jdk -y
ADD https://dlcdn.apache.org/tomcat/tomcat-10/v10.0.22/bin/apache-tomcat-10.0.22.tar.gz .
RUN tar xvzf apache-tomcat-10.0.22.tar.gz
COPY sample.war /usr/local/tomcat/apache-tomcat-10.0.22/webapps/
EXPOSE 8080
CMD ["/usr/local/tomcat/apache-tomcat-10.0.22/bin/catalina.sh" , "run"]
