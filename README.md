# serio-repository
serio maven repository

# maven可以通过以下方式来配置 `pom.xml`:

```XML
<project>

	<properties>
		<version.serio>1.10.6</version.serio>
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
