Lodestone
===========
Lodestone is a fork of the Paper server software with patches from other forks, namely [EmpireCraft][empirecraft] and [Tuinity][tuinity]. It is not meant for widespread use, and is primarily a side-project. You are free to use Lodestone for your server, but support will be limited compared to that of Paper.

It is recommended that you either look into using [Paper][paper] or [Tuinity][tuinity] over using Lodestone. 

How To (Plugin Developers)
------
* See our API patches [here](patches/api)
* Maven Repo (for lodestone-api):
```
This will come with time. For now, you just need to build it locally.
```
* Artifact Information:
```xml
<dependency>
    <groupId>dev.domnian.lodestone</groupId>
    <artifactId>lodestone-api</artifactId>
    <version>1.17-R0.1-SNAPSHOT</version>
    <scope>provided</scope>
</dependency>
 ```

**Or alternatively, with Gradle:**
* Repository:
```
This will come with time. For now, you just need to build it locally.
```
* Artifact:
```groovy
dependencies {
    compileOnly 'dev.domnian.lodestone:lodestone-api:1.17-R0.1-SNAPSHOT'
}
```

How To (Compiling Jar From Source)
------
*The instructions and requirements to compile are the same as [Paper][paper-build].*

To compile Lodestone, you need JDK 16 and an internet connection.

Clone this repo, run `./gradlew applyPatches`, then `./gradlew reobfJar` from your terminal. You can find the compiled jar in the `Lodestone-Server/build/libs` directory.

To get a full list of tasks, run `./gradlew tasks`.

[empirecraft]: https://github.com/starlis/empirecraft
[tuinity]: https://github.com/Tuinity/Tuinity
[paper]: https://github.com/PaperMC/Paper
[paper-build]: https://github.com/PaperMC/Paper/blob/master/README.md#how-to-compiling-jar-from-source