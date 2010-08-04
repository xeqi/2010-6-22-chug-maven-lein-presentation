!SLIDE
#what about clojure?

!SLIDE small
## http://github.com/talios/clojure-maven-plugin
    @@@XML
    <build>
      <plugins>
        <plugin>
          <groupId>com.theoryinpractise</groupId>
          <artifactId>clojure-maven-plugin</artifactId>
          <version>1.3.3</version>
        </plugin>
      </plugins>
    </build>

!SLIDE smbullets
## Goals:
* clojure:compile
* clojure:test
* clojure:run
* clojure:repl
* clojure:swank
* clojure:nailgun

!SLIDE small
    @@@XML
    <build>
      <plugins>
        <plugin>
          <groupId>com.theoryinpractise</groupId>
          <artifactId>clojure-maven-plugin</artifactId>
          <version>1.3.3</version>
        </plugin>
      </plugins>
    </build>

!SLIDE
## Source goes in `src/main/clojure/`
## Tests go in `src/test/clojure/`


!SLIDE
    @@@XML
    <executions>
      <execution>
        <id>compile-clojure</id>
        <phase>compile</phase>
        <goals>
          <goal>compile</goal>
        </goals>
      </execution>
      <execution>
        <id>test-clojure</id>
        <phase>test</phase>
        <goals>
          <goal>test</goal>
        </goals>
      </execution>
    </executions>
