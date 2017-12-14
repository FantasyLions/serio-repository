# serio-repository
serio maven repository

# maven可以通过以下方式来配置 `pom.xml`:

```XML
<project>

	<properties>
		<version.serio>1.0-SNAPSHOT</version.serio>
	</properties>
	
        <repositories>
                <repository>
                    <id>serio-repository</id>
                    <url>https://raw.githubusercontent.com/Fatasylions/serio-repository/master/repository</url>
                </repository>
        </repositories>	

        
	<dependencies>
		<dependency>
			<groupId>com.serio.core</groupId>
			<artifactId>serio-core</artifactId>
			<version>${version.serio}</version>
		</dependency>
	</dependencies>
	
</project>
```

# maven 部署命令

```SHEEL
mvn deploy -DaltDeploymentRepository=serio-core::default::file:D:/DATA/code/serio-repository
```
