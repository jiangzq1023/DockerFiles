#DOCKER-VERSION 1.4.0
FROM jiangzq/java8
#Install tar
RUN yum install -y tar;yum update -y;yum clean all
#ADD tomcate8
ADD apache-tomcat-8.0.15.tar.gz /tmp/
#tar
#RUN tar zxvf /tmp/apache-tomcat-8.0.15.tar.gz
RUN mv /tmp/apache-tomcat-8.0.15 /opt/tomcat8
RUN rm -rf /tmp/*
RUN chmod -R 755 /opt/tomcat8
EXPOSE 8080
CMD /opt/tomcat8/bin/catalina.sh run && tailf /opt/tomcat8/logs/catalina.out

