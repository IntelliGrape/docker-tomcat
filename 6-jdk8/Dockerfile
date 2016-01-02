FROM tomcat:6

RUN echo 'deb http://ftp.de.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list
# Install javac for compilation
RUN apt-get update \
    && apt-get -q -y install openjdk-8-jdk

# Set java home for grailsw to run properly
ENV JAVA_HOME /usr/lib/jvm/java-8-openjdk-amd64

EXPOSE 8080
CMD ["catalina.sh", "run"]
