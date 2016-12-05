FROM tomcat:8.5-jre8

EXPOSE 8080

RUN rm -fr /usr/local/tomcat/webapps/ROOT

COPY server.xml /usr/local/tomcat/conf/server.xml

#  Expectation - calling process will have copied expanded war folder to ./war
COPY war /usr/local/tomcat/webapps/ROOT

# An example run command
#  docker run -p 32800:8080 -p 5702:5701 --env-file ~/twistedX.list --restart=always -d --name twistedX-1.Z-1 jtbdevelopment/twistedX:1.Z
