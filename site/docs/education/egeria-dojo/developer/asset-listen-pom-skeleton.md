<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the Egeria project. -->

Paste this structure into your `pom.xml` class.

```xml

<?xml version="1.0" encoding="UTF-8"?>

<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- Copyright Contributors to the ODPi Egeria project. -->

<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">

    <modelVersion>4.0.0</modelVersion>

    <name>Asset Listen</name>
    <description>
        Listens for events that indicate a new asset has been created and displays information about each one.
    </description>

    <groupId>egeria.dojo</groupId>
    <artifactId>asset-listen</artifactId>
    <version>3.6-SNAPSHOT</version>

    <properties>

        <!-- Level of Java  -->
        <maven.compiler.source>11</maven.compiler.source>
        <maven.compiler.target>11</maven.compiler.target>

        <!-- Platform encoding  -->
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
        <project.reporting.outputEncoding>UTF-8</project.reporting.outputEncoding>

        <!-- Versions of Egeria libraries -->
        <open-metadata.version>3.6-SNAPSHOT</open-metadata.version>

        <!-- Versions of dependent libraries -->
        <logback.version>1.2.10</logback.version>

    </properties>

    <dependencies>

        <dependency>
            <groupId>org.odpi.egeria</groupId>
            <artifactId>open-connector-framework</artifactId>
            <version>${open-metadata.version}</version>
        </dependency>

        <dependency>
            <groupId>org.odpi.egeria</groupId>
            <artifactId>asset-consumer-api</artifactId>
            <version>${open-metadata.version}</version>
        </dependency>

        <dependency>
            <groupId>org.odpi.egeria</groupId>
            <artifactId>asset-consumer-client</artifactId>
            <version>${open-metadata.version}</version>
        </dependency>

        <dependency>
            <groupId>org.odpi.egeria</groupId>
            <artifactId>http-helper</artifactId>
            <version>${open-metadata.version}</version>
        </dependency>

        <dependency>
            <groupId>org.odpi.egeria</groupId>
            <artifactId>kafka-open-metadata-topic-connector</artifactId>
            <version>${open-metadata.version}</version>
        </dependency>

        <dependency>
            <groupId>org.odpi.egeria</groupId>
            <artifactId>csv-file-connector</artifactId>
            <version>${open-metadata.version}</version>
        </dependency>

        <dependency>
            <groupId>ch.qos.logback</groupId>
            <artifactId>logback-classic</artifactId>
            <version>${logback.version}</version>
            <scope>compile</scope>
        </dependency>

    </dependencies>

</project>

```





