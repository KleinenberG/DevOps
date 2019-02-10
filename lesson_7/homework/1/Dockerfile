FROM maven:3-jdk-8-slim
ARG REPO
WORKDIR /prj
RUN apt-get update && apt-get install -y git && \ 
	git clone ${REPO} /prj
CMD ["mvn", "package"]
