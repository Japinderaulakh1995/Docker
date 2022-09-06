FROM redhat/ubi8
RUN mkdir /usr/java/
WORKDIR /usr/java/
RUN yum install java -y 
RUN mkdir /usr/local/tomcat/
WORKDIR /usr/local/tomcat/
ADD https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.65/bin/apache-tomcat-9.0.65.tar.gz .
RUN tar -xvzf apache-tomcat-9.0.65.tar.gz
RUN mv apache-tomcat-9.0.65/* /usr/local/tomcat/
EXPOSE 8080
CMD ["/usr/local/tomcat/catalina.sh", "run"]

#endoffile