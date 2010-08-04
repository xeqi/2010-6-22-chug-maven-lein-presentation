!SLIDE

# Leiningen

!SLIDE bullets
* Project model
* Dependency management
* Builtin actions
* Plugins

!SLIDE small
# Project Model
# project.clj
    (defproject sample-project "0.1.0-SNAPSHOT"
      :dependencies [[org.clojure/clojure "1.1.0]
                     [org.clojure/clojure-contrib "1.1.0"]]
      :dev-dependencies [[swank-clojure "1.2.1"]])

!SLIDE small
# Dependency management
    :dependencies [[org.clojure/clojure "1.1.0]
    :dev-dependencies [[swank-clojure "1.2.1"]]
    :omit-default-repositories true
    :repositories {"java.net"
                   "http://download.java.net/maven/2"}

!SLIDE smbullets
# Builtin Actions

* lein new NAME
* lein deps 
* lein test [TESTS] 
* lein repl 
* lein jar 

!SLIDE 
# No lifecycle
# Deps cached in ~/.m2/
# Deps placed in lib/

!SLIDE
    :source-path "src/"
    :test-path "test/"

!SLIDE
#Plugins

!SLIDE commandline
# $ lein task
# Calls leiningen.task.task
# First arg is Project Model

!SLIDE bullets
* lein swank
* lein run

!SLIDE 
(show example)
