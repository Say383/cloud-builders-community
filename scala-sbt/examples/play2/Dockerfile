FROM openjdk:16.0.2-jdk
ADD target/universal/stage stage
CMD ["stage/bin/play-scala-seed", "-Dplay.http.secret.key=abcdefghijk"]
