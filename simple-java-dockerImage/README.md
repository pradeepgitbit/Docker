# Simple-Java-DockerImage
- A simple java app that runs on docker
---
- java code :

```java

import java.util.Date;

public class Main {
    public static void main(String[] args) {
        Date currentDate = new Date();
        System.out.println("Hello, Docker! Current date: " + currentDate);
    }
}
```
---


- Created the Dockerimage :

```docker
FROM openjdk:27-ea-slim-trixie

WORKDIR /app

COPY src/Main.java /app/Main.java

RUN javac Main.java

CMD [ "java", "Main" ]

```




