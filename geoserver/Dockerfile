FROM tomcat:9.0-jre8
MAINTAINER Ant Somers

#
# Set GeoServer version
#
ENV GEOSERVER_VERSION=2.11.1
ENV GEOSERVER_DATA_DIR="/geoserver_data/data"

#
# Download and install geoserver
#
RUN cd wget --progress=bar:force:noscroll http://sourceforge.net/projects/geoserver/files/GeoServer/${GEOSERVER_VERSION}/geoserver-${GEOSERVER_VERSION}-war.zip \
  && unzip -q geoserver-${GEOSERVER_VERSION}.war.zip -d geoserver \
  && rm geoserver-${GEOSERVER_VERSION}.war \
  && mkdir -p

ENV GEOSERVER_HOME=/usr/share/geoserver
