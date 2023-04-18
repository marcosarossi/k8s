# Toma el Apache Tomcat 8 como imagen base
FROM kwonghung/tomcat:8.0.47-oracle-jdk-1.8

# Establece la variable de entorno de JSAT
ENV JSAT_CONFIG_PATH=/var/jsatconfig/

# Establece la zona horaria
ENV TZ 'America/Buenos_Aires'

# Copia los recursos
COPY ./jsatconfig/ /var/jsatconfig/
COPY ../res/jsat.war /usr/local/tomcat/webapps/jsat.war