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

