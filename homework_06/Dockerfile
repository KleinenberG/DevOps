FROM tomcat:8-jre8-slim
WORKDIR /home
RUN apt-get update && apt-get install -y openjdk-8-jdk maven git && \
	git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /home && \
	mvn package && cp target/*.war /usr/local/tomcat/webapps/
EXPOSE 8080
CMD ["catalina.sh", "run"]	
