simple-gradle-scala
==================

A [giter8][g8] template for scala gradle applications.

Includes

* integration-test source set
* fatJar support

##Usage
Install [giter8][g8], then:

    g8 matlockx/simple-gradle-scala

cd into your new project dir

    chmod +x gradlew
    ./gradlew build

##Gradle Options

###Integration tests
Add tests to src/integration-test/scala
Then run

    ./gradle build -PuseIntegrationTest=true

###FatJar
    ./gradlew build -PcreateFatJar=true

You can also combine these switches.

[g8]: http://github.com/n8han/giter8#readme