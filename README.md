# springboot-docker-kotlin
Project created for Study SpringBoot + Kotlin + Docker

# Building Docker image
``` ./gradlew clean build docker```

# Running Docker Container
```docker run --name springboot-kotlin -d --memory=100m -p 8080:8080 augustomarinho/study:springboot-docker-kotlin-0.0.1-SNAPSHOT```