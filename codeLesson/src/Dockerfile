FROM tomcat:9.0.53-jdk11-openjdk

# Elimina la aplicación de ejemplo de Tomcat
RUN rm -rf /usr/local/tomcat/webapps/ROOT

# Copia tu archivo WAR en el directorio webapps de Tomcat
COPY build/libs/codeLesson-0.0.1-SNAPSHOT.war /usr/local/tomcat/webapps/ROOT.war

# Expone el puerto 8080
EXPOSE 8080

CMD ["catalina.sh", "run"]
