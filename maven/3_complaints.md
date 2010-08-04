!SLIDE
# Complaints

!SLIDE
# It's complicated

!SLIDE
# I don't trust the internet for dependencies 

!SLIDE
## `settings.xml`
    @@@XML
    <project>
      ...
      <repositories>
        <repository>
          <id>my-internal-site</id>
          <url>http://myserver/repo</url>
        </repository>
      </repositories>
      ...
    </project>

!SLIDE
# I hate XML

!SLIDE

# polyglot-maven
## http://polyglot.sonatype.org/clojure.html

!SLIDE smaller
    @@@clojure
    (defproject main "org.sonatype:mvn-clojure-test:1.0-SNAPSHOT"
      :dependencies
        [["org.clojure:clojure-lang:1.1.0-alpha-SNAPSHOT"]
         ["org.clojure:clojure-contrib:1.0-SNAPSHOT"]]
      :test-dependencies [["org.junit:junit:4.2"]])
