FROM tomcat:6

# Install javac for compilation
RUN apt-get update \
    && apt-get -q -y install openjdk-7-jdk

# Set java home for grailsw to run properly
ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64

EXPOSE 8080
CMD ["catalina.sh", "run"]
