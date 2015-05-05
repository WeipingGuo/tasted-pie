# tasted-pie

A sample project to show how to use git as Maven repository.


## build step

```
mvn clean deploy
```
This will build and upload files to github


## How to use

### add github repository to the pom.xml
```
<repository>
	<id>tested-pi-mvn-repo</id>
    <url>https://raw.github.com/WeipingGuo/tasted-pie/mvn-repo/</url>
    <snapshots>
    	<enabled>true</enabled>
        <updatePolicy>always</updatePolicy>
    </snapshots>
</repository>
```

### add dependency to pom.xml
```
<dependency>
		<groupId>com.gmail.wguo1990</groupId>
  		<artifactId>tasted-pie</artifactId>
  		<version>0.0.1-SNAPSHOT</version>
</dependency>
```
