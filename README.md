# Setup

```declarative
gradle init --use-defaults --type java-application
```
The above setup basic gradle project

```agsl
gradlew build
``` 
To prepare a jar which is execuatble, you need to setup manifest property in build.gradle
```grovy
jar {
    manifest {
        attributes(
            'Main-Class': 'org.example.Main'
        )
    }
}

```
The above command can build your project

```agsl
gradlew jar
```
The above command creates a new jar file in `build/libs`folder

```agsl
java -jar C:\Users\saisu\OneDrive\Desktop\2026-SST-LEARN\GradleProjectUsingCli\app\build\libs\app-1.0-SNAPSHOT.jar
```
The above command will execute your code
