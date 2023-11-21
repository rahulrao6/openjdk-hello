# Build stage
FROM openjdk:latest as builder
COPY HelloWorld.java .
RUN javac HelloWorld.java

# Distroless stage
FROM gcr.io/distroless/java:latest
COPY --from=builder HelloWorld.class /
CMD ["HelloWorld"]
