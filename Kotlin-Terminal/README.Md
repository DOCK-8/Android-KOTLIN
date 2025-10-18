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
The next tool for our development is gradle. It is a dependency management and an easy option for installing dependencies in a project to compile our app. This tool is similar to maven, which is a well-known reference in web development.
To install it, we navigate to the [Gradle Web Page](https://gradle.org/releases/) and install the Gradle Version Package.
```bash
# We make folder where gradle will be installed
mkdir -p /opt/gradle
# We uncompress in the folder created (Recommend that we are superusers)
unzip -d /opt/gradle $RUTA/gradle-version.zip
# We create environment variable
export PATH=$PATH:/opt/gradle/gradle-version/bin
# Verificate
gradle -v
```
##  SDK
These are tools used to create mobile apps and compile them with the necessary Android dependencies. The SDK includes tools for debugging, compiling, and other essential tasks needed to work with Android Compose.
So, we go to the [Android command line tools](https://developer.android.com/studio#command-line-tools-only) page and select the  platform compatible with our operating system.
```bash
# Download package
# Create the folder where SDK will be installed
mkdir -p $HOME/Android/Sdk/
# Create environment path for this space
export ANDROID_HOME=$HOME/Android/Sdk/
# Uncompress the dowloaded file and adjust the folder structure
unzip -d $ANDROID_HOME path_of_download/commandlinetools-linux-version_latest.zip
# The folder structure
# ├── cmdline-tools
# │   └── latest
# │       ├── bin
# │       ├── lib
# │       ├── Another files ...
# Create the path
export PATH=$PATH:$ANDROID_HOME/cmdline-tools/latest/bin
#Verify
sdkmanager --list

```
