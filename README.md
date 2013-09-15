Liferay Layout Parent
=====================

Maven parent pom for Liferay Layout plugins.

Use this parent in your Liferay Layout project *pom.xml*:

```xml
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<artifactId>4-2-1-columns-layouttpl</artifactId>
	<packaging>war</packaging>
	<name>4-2-1 Columns (70/30)</name>
	<version>1.1</version>

	<parent>
		<groupId>eu.prvaci</groupId>
		<artifactId>layout-parent</artifactId>
		<version>1.0</version>
	</parent>
...
```

The only property, that needs to be set up is:

```xml
<properties>
	<liferay.auto.deploy.dir>~/Liferay/liferay-portal-6.1.2-ce-ga3/deploy/</liferay.auto.deploy.dir>
</properties>
```

Then you can simply run:

```bash
mvn clean package liferay:deploy
```