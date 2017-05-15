FROM ubuntu:16.04

RUN apt-get update \
	&& apt-get install -y \
		libapr1 \
		libaprutil1 \
		libaprutil1-ldap \
		libapr1-dev \
		libaprutil1-dev \
		liblua5.2-0 \
		libnghttp2-14 \
		libssl1.0.0 \
		libxml2 \
                apache2 \
                php7.0 \
                php7.0-mysql \
                libapache2-mod-php7.0 \
&& rm -r /var/lib/apt/lists/*

COPY httpd-foreground /usr/local/bin/

EXPOSE 80
CMD ["httpd-foreground"]
