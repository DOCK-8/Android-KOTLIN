# JETPACK-COMPOSE
initially, we may need to have *Java* and the dependency management tool *Gradle*
## JAVA
We navigate to the [Java web page](https://www.java.com/es/download/linux_manual.jsp) and install the Java compressed package 
Next step, we uncompress the _Java Package_ into the path that the system calls Java.
Verificate
```bash
java -v
```
## GRADLE
The next tool for our development is gradle. It is a dependency management and a easy option for installing dependencies in a project to compile our app. this tool is similar to maven, which is a well-known reference in web development.
The install, we navigate to the [Gradle Web Page](https://gradle.org/releases/) and install the Gradle Version Package.
```bash
# We make folder to grabe will be
mkdir -p /opt/gradle
# We uncompress in the folder created (_Recommend that we are superusers_)
unzip -d /opt/gradle $RUTA/gradle-version/
# We create environmet variable
export PATH=$PATH:/opt/gradle/gradle-version/bin
```
