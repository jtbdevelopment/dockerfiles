FROM tomcat:8.5-jre8

EXPOSE 8080

RUN rm -fr /usr/local/tomcat/webapps/ROOT

#  Expectation - derived dockerfile will copy or add expanded war files to root
#  COPY war-1.0-SNAPSHOT /usr/local/tomcat/webapps/ROOT