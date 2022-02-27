# program-cleverly

nonsense becomes serious 🦖 ...


public class energie { public static void main(String s[])
{ System.out.println("energiemonitor ..."); } }public class energie { public static void main(String s[])
{ System.out.println("energiemonitor ..."); } }public class energie { public static void main(String s[])
{ System.out.println("energiemonitor ..."); } }
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>de.meinefirma.meinprojekt</groupId>
  <artifactId>OzarkJavaxMvcMitJetty</artifactId>
  <version>1.0-SNAPSHOT</version>
  <packaging>war</packaging>
  <name>${project.artifactId}</name>
  <properties>
    <jetty.version>9.4.7.v20170914</jetty.version>
    <jersey.version>2.26</jersey.version>
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
  </properties>
  <build>
    <finalName>${project.artifactId}</finalName>
    <plugins>
      <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-compiler-plugin</artifactId>
        <version>3.7.0</version>
        <configuration>
          <source>1.8</source>
          <target>1.8</target>
        </configuration>
      </plugin>
      <plugin>
        <groupId>org.eclipse.jetty</groupId>
        <artifactId>jetty-maven-plugin</artifactId>
        <version>${jetty.version}</version>
        <configuration>
          <jvmArgs>--add-modules java.xml.bind</jvmArgs>
          <scanIntervalSeconds>10</scanIntervalSeconds>
          <webApp>
            <contextPath>/${project.artifactId}</contextPath>
          </webApp>
          <httpConnector>
            <port>8080</port>
          </httpConnector>
        </configuration>
      </plugin>
    </plugins>
  </build>
  <dependencies>
    <dependency>
      <groupId>javax</groupId>
      <artifactId>javaee-api</artifactId>
      <version>7.0</version>
      <scope>provided</scope>
    </dependency>
    <dependency>
      <groupId>javax.mvc</groupId>
      <artifactId>javax.mvc-api</artifactId>
      <version>1.0-edr2</version>
    </dependency>
    <dependency>
      <groupId>org.glassfish.ozark</groupId>
      <artifactId>ozark</artifactId>
      <version>1.0.0-m02</version>
    </dependency>
    <dependency>
      <groupId>org.glassfish.jersey.containers</groupId>
      <artifactId>jersey-container-servlet</artifactId>
      <version>${jersey.version}</version>
    </dependency>
    <dependency>
      <groupId>org.glassfish.jersey.ext.cdi</groupId>
      <artifactId>jersey-cdi1x</artifactId>
      <version>${jersey.version}</version>
    </dependency>
    <dependency>
      <groupId>org.glassfish.jersey.ext</groupId>
      <artifactId>jersey-bean-validation</artifactId>
      <version>${jersey.version}</version>
    </dependency>
    <dependency>
      <groupId>org.glassfish.jersey.inject</groupId>
      <artifactId>jersey-hk2</artifactId>
      <version>${jersey.version}</version>
    </dependency>
    <dependency>
      <groupId>org.glassfish.hk2</groupId>
      <artifactId>hk2-api</artifactId>
      <version>2.5.0-b59</version>
    </dependency>
    <dependency>
      <groupId>javax.enterprise</groupId>
      <artifactId>cdi-api</artifactId>
      <version>2.0</version>
    </dependency>
    <dependency>
      <groupId>org.jboss.weld.servlet</groupId>
      <artifactId>weld-servlet-core</artifactId>
      <version>2.4.4.Final</version>
    </dependency>
    <dependency>
      <groupId>org.eclipse.jetty</groupId>
      <artifactId>jetty-servlet</artifactId>
      <version>${jetty.version}</version>
    </dependency>
  </dependencies>
</project>
