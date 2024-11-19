FROM tomcat:10-jdk21
LABEL "Project"="Vprofile"
LABEL "Author"="MahdiSavoji"

# Remove default webapps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy WAR file to Tomcat webapps
COPY target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080
CMD ["catalina.sh", "run"]

WORKDIR /usr/local/tomcat/
VOLUME /usr/local/tomcat/webapps
