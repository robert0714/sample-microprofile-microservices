https://piotrminkowski.com/2020/12/14/microprofile-java-microservices-on-wildfly/
# Readme
Finally, we just need to execute the following command to build and run our “Fat JAR” application on WildFly.

```bash 
mvn package wildfly-jar:run
````

The application employee-service is available on http://localhost:8080/
Then let’s call the endpoint http://localhost:9990/metrics

After starting the application we may access OpenAPI documentation by calling http://localhost:8080/openapi


## Deploy MicroProfile microservices on OpenShift


```bash
mvn oc:deploy -P bootable-jar-openshift
```