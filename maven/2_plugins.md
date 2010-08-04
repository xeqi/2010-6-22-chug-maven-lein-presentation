!SLIDE
# Other Plugins

!SLIDE
# Standalone Executable Jar

!SLIDE small
    @@@XML
    <plugin>
      <artifactId>maven-assembly-plugin</artifactId>
      <configuration>
        <archive>
          <manifest>
            <mainClass>example.core</mainClass>
          </manifest>
        </archive>
        <descriptorRefs>
          <descriptorRef>
            jar-with-dependencies
          </descriptorRef>
        </descriptorRefs>
      </configuration>
    </plugin>

!SLIDE code small
## mvn assembly:assembly
## java -jar target/example-0.1-jar-with-dependencies.jar

!SLIDE
# OSX bundle

!SLIDE small
    @@@XML
    <plugin>
      <groupId>org.codehaus.mojo</groupId>
      <artifactId>osxappbundle-maven-plugin</artifactId>
      <version>1.0-alpha-1</version>
      <configuration>
        <mainClass>example.core</mainClass>
      </configuration>
    </plugin>

!SLIDE
# Selenium
## (automated testing against a web app)

!SLIDE small
    @@@XML
    <plugin>
      <groupId>org.codehaus.mojo</groupId>
      <artifactId>selenium-maven-plugin</artifactId>
      <executions>
        <execution>
          <id>start</id>
          <phase>pre-integration-test</phase>
          <goals>
            <goal>start-server</goal>
          </goals>
          <configuration>
            <background>true</background>
          </configuration>
        </execution>
        <execution>
          <id>stop</id>
          <phase>post-integration-test</phase>
          <goals>
            <goal>stop-server</goal>
          </goals>
        </execution>
      </executions>
    </plugin>

!SLIDE
# I want to do `X`

!SLIDE
# Search the internet
## lots of plugins available

!SLIDE bullets
* jruby
* gae
* gwt

!SLIDE
## (show example)
