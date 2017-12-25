# serio-repository
serio maven repository

# maven可以通过以下方式来配置 `pom.xml`:

```XML
<project>

	<properties>
		<version.serio>1.0.0</version.serio>
        <version.jsonrpc4j>1.6.0</version.jsonrpc4j>
	</properties>
	
        <repositories>
                <repository>
                    <id>serio-repository</id>
                    <url>https://raw.githubusercontent.com/fantasylion/serio-repository/master</url>
                </repository>
        </repositories>	

        
	<dependencies>
		
        <dependency>
			<groupId>com.serio</groupId>
			<artifactId>serio-core</artifactId>
			<version>${version.serio}</version>
		</dependency>


        <dependency>
            <groupId>com.serio</groupId>
            <artifactId>jsonrpc4j</artifactId>
            <version>${version.jsonrpc4j}</version>
        </dependency>
	</dependencies>

    
	
</project>
```

# maven 部署命令

```SHEEL
mvn deploy -DaltDeploymentRepository=serio-core::default::file:D:/DATA/code/serio-repository
```
