FROM httpd:latest

#  Expected as part of run host container will mount a volume overlaying /usr/local/apache2/conf
#  which will contain:
#    extra/httpd-vhosts.conf to define remappings
#    extra/server.key for SSL key
#    extra/server.crt for SSL crt file
#    extra/server-ca.crt for intermmediate crt file

#  These should be exposed directly as 80 and 443
EXPOSE 80 443

COPY httpd.conf /usr/local/apache2/conf/httpd.conf

# An example run command
# Example vhosts file in this package
#  docker run -d --restart=always --name twistedapache -v PATHTO/apache2/conf/httpd-vhosts.conf:/usr/local/apache2/conf/extra/httpd-vhosts.conf -v PATHTO/apache2/conf/server.key:/usr/local/apache2/conf/server.key -v PATHTO/apache2/conf/server.crt:/usr/local/apache2/conf/server.crt -v  PATHTO/apache2/conf/server-ca.crt:/usr/local/apache2/conf/server-ca.crt -p 80:80 -p 443:443 jtbdevelopment/twistedapache

