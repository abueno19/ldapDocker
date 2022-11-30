FROM php:7.4-apache
RUN apt-get update -y --fix-missing && apt-get upgrade -y
RUN apt-get install -y libldb-dev libldap2-dev  ldap-utils 
RUN a2enmod authnz_ldap


COPY conf/000-default.conf /etc/apache2/sites-available/000-default.conf
