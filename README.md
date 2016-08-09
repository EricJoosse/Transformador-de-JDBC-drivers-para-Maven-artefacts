# Transformador de JDBC drivers para Maven artifacts

Até agora apenas os seguintes drivers já foram transformados : 
* Firebird
* Oracle


Estes 2 Maven artifacts foram "deployed" para o seguinte Remote Maven Repository : 

https://github.com/EricJoosse/Remote-Maven-Repository-de-JDBC-Drivers 

Estes Maven artifacts podem ser referenciados em arquivos pom.xml da seguinte forma : 
```
  <repositories>
    <repository>
        <id>Remote-Maven-Repository-com-JDBC-Drivers</id>
        <url>https://raw.github.com/EricJoosse/Remote-Maven-Repository-com-JDBC-Drivers/mvn-repo/</url>
        <snapshots>
            <enabled>true</enabled>
            <updatePolicy>always</updatePolicy>
        </snapshots>
    </repository>
  </repositories>

  <dependencies>
    <dependency>
    	<groupId>oracle.jdbc</groupId>
    	<artifactId>jdbc-oracle</artifactId>
    	<version>10.2.0.5.0</version>
    </dependency>
    <dependency>
    	<groupId>org.firebirdsql.jdbc</groupId>
    	<artifactId>jaybird-full</artifactId>
    	<version>2.2.10</version>
    </dependency>
  </dependencies>
```
