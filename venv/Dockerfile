FROM tomcat:9.0
RUN apt update
RUN apt install git -y
RUN apt install maven -y
WORKDIR /home/nealick/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /home/nealick/boxfuse-sample-java-war-hello/
RUN mvn package
WORKDIR /home/nealick/boxfuse-sample-java-war-hello/
RUN cp hello-1.0.war /var/lib/tomcat9/webapps/
