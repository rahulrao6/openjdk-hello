FROM registry.access.redhat.com/ubi8/openjdk-11:latest
COPY HelloWorld.java .
RUN javac HelloWorld.java
CMD ["java", "HelloWorld"]
EXPOSE 8080
