FROM openjdk:27-ea-slim-trixie

WORKDIR /app

COPY src/Main.java /app/Main.java

RUN javac Main.java

CMD [ "java", "Main" ]