simple-gradle-scala
==================

A [giter8][g8] template for scala gradle applications.

Includes

* integration-test source set
* fatJar support
* app support
* heroku support

##Usage
Install [giter8][g8], then:

    g8 matlockx/simple-gradle-scala

cd into your new project dir

    ./gradlew build

##Gradle Options

###Integration tests
Add tests to src/integration-test/scala
Then run

    ./gradle build -PuseIntegrationTest=true

###FatJar
    ./gradlew build -PcreateFatJar=true

###App Support
	./gradlew installApp
	./build/install/[projectName]/bin/[projectName]

###Heroku
When you have an heroku account, then you could create a heroku app with your created project dir. After pushing your changes to heroku the app should run immediately. How does it work? There is a gradle task 'stage' which will call installApp. The output is used by foreman and the Procfile which is also located in your new project.

[g8]: http://github.com/n8han/giter8#readme