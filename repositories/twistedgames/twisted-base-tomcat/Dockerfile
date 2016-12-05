FROM tomcat:8.5-jre8

EXPOSE 8080

RUN rm -fr /usr/local/tomcat/webapps/ROOT

COPY server.xml /usr/local/tomcat/conf/server.xml

#  Expectation - calling process will have copied expanded war folder to ./war
COPY war /usr/local/tomcat/webapps/ROOT