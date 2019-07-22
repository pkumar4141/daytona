FROM centos
USER root
ENV XY=jar
ENV FINVER=0.0.1-20190720.021339-1
RUN yum install wget java tomcat -y
RUN mkdir -p /var/lib/tomcat/api
WORKDIR /var/lib/tomcat/api
RUN cd /var/lib/tomcat/api && wget http://10.142.0.17:8081/repository/devops_snapshot/co/daytona/test/devops/0.0.1-SNAPSHOT/devops-$FINVER.\jar
ENTRYPOINT java -jar devops-$FINVER.jar


