# SOvaadinpom
## A POM file for Vaadin projects.

This POM file can be used as a parent POM for your Vaadin project.
You can build a war or jar file of your project.
All necessary jar file dependencies are included.

The version of this POM file always matches with the supported Vaadin release version.

The Java version is the current LTS version - Java 21.

It has Jetty integration. So, you can run it from the IDE or from a terminal.
```shell
mvn jetty:run
```

Just like any other Vaadin project, you can create the production build.
```shell
mvn clean install -Pproduction
```

Just use this as the parent POM like:
```xml
  <parent>
    <groupId>com.storedobject</groupId>
    <artifactId>so-vaadinpom</artifactId>
    <version>24.7.1</version>
    <relativePath/>
  </parent>
```
Also, include this in your repositories section:
```xml
<repositories>
    <repository>
        <id>so-maven</id>
        <url>https://storedobject.com/maven</url>
    </repository>
</repositories>
```