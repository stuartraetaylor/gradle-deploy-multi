# Gradle deploy multiple webapps to Wildfly

Basic project that uses Gradle to deploy two webapps to Wildfly.

The deployment works one webapp at a time, but fails with multiple webapps.

## Working Example - deploy one webapp at a time

```
./gradlew -Pwildfly.user=myuser -Pwildfly.password=mypass :webapp_1:wildflyDeploy
./gradlew -Pwildfly.user=myuser -Pwildfly.password=mypass :webapp_2:wildflyDeploy
```

## Broken Example - deploy multiple webapps
```
./gradlew -Pwildfly.user=myuser -Pwildfly.password=mypass wildflyDeploy

```
