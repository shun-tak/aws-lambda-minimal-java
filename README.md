# AWS Lambda minimal Java

## Build

with maven
```
cd hello
mvn package
```

with gradle
```
./gradlew hello:shadowJar
```

## AWS Lambda settings

- runtime: Java8
- function package
  - maven build: `hello/target/lambda-java-example-1.0-SNAPSHOT.jar`
  - gradle build: `hello/build/libs/hello-1.0-SNAPSHOT-all.jar`
- handler: `example.Hello::myHandler`

## Test

Input: `1`
Expected output: `"1"`
