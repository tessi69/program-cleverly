# program-cleverly

nonsense becomes serious 🦖 ...

 Trip Time, RTT) ab [CBC+10]. Die RTT ist die Zeit, die ein Paket im Netzwerk von einer Quelle zum Ziel und zurück benötigt. Je nach Netzwerkanbindung variiert diese Zeit. Eine konkrete Messung der verbrauchten Energie beim Senden von Daten von einem Mobiltelefon wurde in [CBC+10] durch- geführt. In einem WLAN mit einer RTT von 25 ms verbraucht das Hochladen von 100 kB laut den Autoren 576 mJ. Bei derselben Verbindung und einer RTT von 50 ms erfordere die Aktion mit 989 mJ bereits fast die doppelte Energie. In einer mobilen Netzwerkverbindung über UMTS, bei der eine RTT von 220 ms gemessen wurde, würden sogar schon 2.762 mJ an Energie für das Hochladen von 100 kB fällig, schreiben die Verfasser der Publikation.
Neben der Netzwerkanbindung ist natürlich auch Wissen über die Größe der zu übertragenden Daten notwendig, um den Übertragungsaufwand errechnen zu können. Dazu bestimmt die Offloading- Komponente alle Objekte, welche von der Methode, die ausgelagert werden soll, verwendet werden. Die Autoren setzen die gefundenen Objekte daraufhin mit ihrem Serialisierer in eine plattformunabhängige Form um. Die Größe dieses serialisierten Objekts kann nun für die Berechnung der Übertragungskosten genutzt werden.
 
 Der energetische Aufwand zum lokalen Ausführen einer Methode wird hauptsächlich von der Zeit bestimmt, die diese bei der Ausführung auf dem lokalen Prozessor verbraucht. Ein einfacher Ansatz zum Finden dieser Größe ist das einfache Messen der Ausführungszeit von Methoden. Die Offloading- Komponente kann vor jeder Methodenausführung eine Messung deren Laufzeit starten, um beim nächsten Aufruf auf das Ergebnis davon zurückzugreifen. Je mehr Messdaten zur Verfügung stehen, desto genauer wird statistisch die Vorhersage der nächsten Ausführungsdauer einer Methode. Beim ersten Aufruf einer Methode liefert dieser Ansatz jedoch noch keine Daten. Dabei könnte bereits das Wissen über eine Minimaldauer die Offloading-Komponente dazu verleiten, einen Programmteil auszulagern. Dauert dieser länger, als berechnet, wird sogar mehr Energie gespart, als errechnet. Nur wenn die tatsächliche Dauer unter der berechneten liegt, kann durch Code-Offloading ein energetischer Nachteil entstehen. Das Finden der Ausführungszeit vor der ersten Ausführung einer Methode, nur auf Grundlage der zu diesem Zeitpunkt verfügbaren Daten, ist der zentrale Gegenstand dieser Arbeit.


@newcoding
public class energie { public static void main(String s[])
{ System.out.println("energiemonitor ..."); } }public class energie { public static void main(String s[])
{ System.out.println("energiemonitor ..."); } }public class energie { public static void main(String s[])
{ System.out.println("energiemonitor ..."); } }
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <'groupId>de.meinefirma.meinprojekt</groupId>
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
      
           < name: 'tessi69 >
                    
                    <project xmlns="http://maven.apache.org/POM/4.1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.1.2 http://maven.apache.org/xsd/maven-4.1.2.xsd">
                    
           < plugin>
 <build>
          <finalName>${project.artifacId}</finalName>
          <plugins>
            <groupId>org.apache.maven,plugins</groupId>
                   <artifactId>maven-compiler-plugin</artifactId>
                   <version>3.7.2</version>
                   <configuration>
                            <source>1.9</source>
                   <target>1.9</target>
                   </configuration>
          </plugin>
            
                    </ name: tessi69'
                    
               
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
<a href://www.alleswirdgut.de>
</a>

..........
