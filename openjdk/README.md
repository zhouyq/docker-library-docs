<!--

********************************************************************************

WARNING:

    DO NOT EDIT "openjdk/README.md"

    IT IS AUTO-GENERATED

    (from the other files in "openjdk/" combined with a set of templates)

********************************************************************************

-->

**Note:** this is the "per-architecture" repository for the `arm64v8` builds of [the `openjdk` official image](https://hub.docker.com/_/openjdk) -- for more information, see ["Architectures other than amd64?" in the official images documentation](https://github.com/docker-library/official-images#architectures-other-than-amd64) and ["An image's source changed in Git, now what?" in the official images FAQ](https://github.com/docker-library/faq#an-images-source-changed-in-git-now-what).

# **DEPRECATION NOTICE**

This image is officially deprecated and all users are recommended to find and use suitable replacements ASAP. Some examples of other Official Image alternatives (listed in alphabetical order with no intentional or implied preference):

-	[`amazoncorretto`](https://hub.docker.com/_/amazoncorretto)
-	[`eclipse-temurin`](https://hub.docker.com/_/eclipse-temurin)
-	[`ibm-semeru-runtimes`](https://hub.docker.com/_/ibm-semeru-runtimes)
-	[`ibmjava`](https://hub.docker.com/_/ibmjava)
-	[`sapmachine`](https://hub.docker.com/_/sapmachine)

See [docker-library/openjdk#505](https://github.com/docker-library/openjdk/issues/505) for more information.

The only tags which will continue to receive updates beyond July 2022 will be Early Access builds (which are sourced from [jdk.java.net](https://jdk.java.net/)), as those are not published/supported by any of the above projects.

# Quick reference

-	**Maintained by**:  
	[the Docker Community](https://github.com/docker-library/openjdk)

-	**Where to get help**:  
	[the Docker Community Forums](https://forums.docker.com/), [the Docker Community Slack](https://dockr.ly/slack), or [Stack Overflow](https://stackoverflow.com/search?tab=newest&q=docker)

# Supported tags and respective `Dockerfile` links

(See ["What's the difference between 'Shared' and 'Simple' tags?" in the FAQ](https://github.com/docker-library/faq#whats-the-difference-between-shared-and-simple-tags).)

## Simple Tags

-	[`20-ea-6-jdk-oraclelinux8`, `20-ea-6-oraclelinux8`, `20-ea-jdk-oraclelinux8`, `20-ea-oraclelinux8`, `20-jdk-oraclelinux8`, `20-oraclelinux8`, `20-ea-6-jdk-oracle`, `20-ea-6-oracle`, `20-ea-jdk-oracle`, `20-ea-oracle`, `20-jdk-oracle`, `20-oracle`](https://github.com/docker-library/openjdk/blob/7be88afe2fd7b6f4b28c7434a9c2d409c53fa0e3/20/jdk/oraclelinux8/Dockerfile)
-	[`20-ea-6-jdk-oraclelinux7`, `20-ea-6-oraclelinux7`, `20-ea-jdk-oraclelinux7`, `20-ea-oraclelinux7`, `20-jdk-oraclelinux7`, `20-oraclelinux7`](https://github.com/docker-library/openjdk/blob/7be88afe2fd7b6f4b28c7434a9c2d409c53fa0e3/20/jdk/oraclelinux7/Dockerfile)
-	[`20-ea-6-jdk-bullseye`, `20-ea-6-bullseye`, `20-ea-jdk-bullseye`, `20-ea-bullseye`, `20-jdk-bullseye`, `20-bullseye`](https://github.com/docker-library/openjdk/blob/7be88afe2fd7b6f4b28c7434a9c2d409c53fa0e3/20/jdk/bullseye/Dockerfile)
-	[`20-ea-6-jdk-slim-bullseye`, `20-ea-6-slim-bullseye`, `20-ea-jdk-slim-bullseye`, `20-ea-slim-bullseye`, `20-jdk-slim-bullseye`, `20-slim-bullseye`, `20-ea-6-jdk-slim`, `20-ea-6-slim`, `20-ea-jdk-slim`, `20-ea-slim`, `20-jdk-slim`, `20-slim`](https://github.com/docker-library/openjdk/blob/7be88afe2fd7b6f4b28c7434a9c2d409c53fa0e3/20/jdk/slim-bullseye/Dockerfile)
-	[`20-ea-6-jdk-buster`, `20-ea-6-buster`, `20-ea-jdk-buster`, `20-ea-buster`, `20-jdk-buster`, `20-buster`](https://github.com/docker-library/openjdk/blob/7be88afe2fd7b6f4b28c7434a9c2d409c53fa0e3/20/jdk/buster/Dockerfile)
-	[`20-ea-6-jdk-slim-buster`, `20-ea-6-slim-buster`, `20-ea-jdk-slim-buster`, `20-ea-slim-buster`, `20-jdk-slim-buster`, `20-slim-buster`](https://github.com/docker-library/openjdk/blob/7be88afe2fd7b6f4b28c7434a9c2d409c53fa0e3/20/jdk/slim-buster/Dockerfile)
-	[`19-ea-31-jdk-oraclelinux8`, `19-ea-31-oraclelinux8`, `19-ea-jdk-oraclelinux8`, `19-ea-oraclelinux8`, `19-jdk-oraclelinux8`, `19-oraclelinux8`, `19-ea-31-jdk-oracle`, `19-ea-31-oracle`, `19-ea-jdk-oracle`, `19-ea-oracle`, `19-jdk-oracle`, `19-oracle`](https://github.com/docker-library/openjdk/blob/e3497a96e0b6c614bdd306d7d47ba32314545a48/19/jdk/oraclelinux8/Dockerfile)
-	[`19-ea-31-jdk-oraclelinux7`, `19-ea-31-oraclelinux7`, `19-ea-jdk-oraclelinux7`, `19-ea-oraclelinux7`, `19-jdk-oraclelinux7`, `19-oraclelinux7`](https://github.com/docker-library/openjdk/blob/e3497a96e0b6c614bdd306d7d47ba32314545a48/19/jdk/oraclelinux7/Dockerfile)
-	[`19-ea-31-jdk-bullseye`, `19-ea-31-bullseye`, `19-ea-jdk-bullseye`, `19-ea-bullseye`, `19-jdk-bullseye`, `19-bullseye`](https://github.com/docker-library/openjdk/blob/e3497a96e0b6c614bdd306d7d47ba32314545a48/19/jdk/bullseye/Dockerfile)
-	[`19-ea-31-jdk-slim-bullseye`, `19-ea-31-slim-bullseye`, `19-ea-jdk-slim-bullseye`, `19-ea-slim-bullseye`, `19-jdk-slim-bullseye`, `19-slim-bullseye`, `19-ea-31-jdk-slim`, `19-ea-31-slim`, `19-ea-jdk-slim`, `19-ea-slim`, `19-jdk-slim`, `19-slim`](https://github.com/docker-library/openjdk/blob/e3497a96e0b6c614bdd306d7d47ba32314545a48/19/jdk/slim-bullseye/Dockerfile)
-	[`19-ea-31-jdk-buster`, `19-ea-31-buster`, `19-ea-jdk-buster`, `19-ea-buster`, `19-jdk-buster`, `19-buster`](https://github.com/docker-library/openjdk/blob/e3497a96e0b6c614bdd306d7d47ba32314545a48/19/jdk/buster/Dockerfile)
-	[`19-ea-31-jdk-slim-buster`, `19-ea-31-slim-buster`, `19-ea-jdk-slim-buster`, `19-ea-slim-buster`, `19-jdk-slim-buster`, `19-slim-buster`](https://github.com/docker-library/openjdk/blob/e3497a96e0b6c614bdd306d7d47ba32314545a48/19/jdk/slim-buster/Dockerfile)
-	[`18.0.1.1-jdk-oraclelinux8`, `18.0.1.1-oraclelinux8`, `18.0.1-jdk-oraclelinux8`, `18.0.1-oraclelinux8`, `18.0-jdk-oraclelinux8`, `18.0-oraclelinux8`, `18-jdk-oraclelinux8`, `18-oraclelinux8`, `jdk-oraclelinux8`, `oraclelinux8`, `18.0.1.1-jdk-oracle`, `18.0.1.1-oracle`, `18.0.1-jdk-oracle`, `18.0.1-oracle`, `18.0-jdk-oracle`, `18.0-oracle`, `18-jdk-oracle`, `18-oracle`, `jdk-oracle`, `oracle`](https://github.com/docker-library/openjdk/blob/dd758df145819316fbe6cf4c53a95bfa27c62ae5/18/jdk/oraclelinux8/Dockerfile)
-	[`18.0.1.1-jdk-oraclelinux7`, `18.0.1.1-oraclelinux7`, `18.0.1-jdk-oraclelinux7`, `18.0.1-oraclelinux7`, `18.0-jdk-oraclelinux7`, `18.0-oraclelinux7`, `18-jdk-oraclelinux7`, `18-oraclelinux7`, `jdk-oraclelinux7`, `oraclelinux7`](https://github.com/docker-library/openjdk/blob/77713ecc13f1480f3fe2b53fe03f2afb12727c74/18/jdk/oraclelinux7/Dockerfile)
-	[`18.0.1.1-jdk-bullseye`, `18.0.1.1-bullseye`, `18.0.1-jdk-bullseye`, `18.0.1-bullseye`, `18.0-jdk-bullseye`, `18.0-bullseye`, `18-jdk-bullseye`, `18-bullseye`, `jdk-bullseye`, `bullseye`](https://github.com/docker-library/openjdk/blob/dd758df145819316fbe6cf4c53a95bfa27c62ae5/18/jdk/bullseye/Dockerfile)
-	[`18.0.1.1-jdk-slim-bullseye`, `18.0.1.1-slim-bullseye`, `18.0.1-jdk-slim-bullseye`, `18.0.1-slim-bullseye`, `18.0-jdk-slim-bullseye`, `18.0-slim-bullseye`, `18-jdk-slim-bullseye`, `18-slim-bullseye`, `jdk-slim-bullseye`, `slim-bullseye`, `18.0.1.1-jdk-slim`, `18.0.1.1-slim`, `18.0.1-jdk-slim`, `18.0.1-slim`, `18.0-jdk-slim`, `18.0-slim`, `18-jdk-slim`, `18-slim`, `jdk-slim`, `slim`](https://github.com/docker-library/openjdk/blob/dd758df145819316fbe6cf4c53a95bfa27c62ae5/18/jdk/slim-bullseye/Dockerfile)
-	[`18.0.1.1-jdk-buster`, `18.0.1.1-buster`, `18.0.1-jdk-buster`, `18.0.1-buster`, `18.0-jdk-buster`, `18.0-buster`, `18-jdk-buster`, `18-buster`, `jdk-buster`, `buster`](https://github.com/docker-library/openjdk/blob/dd758df145819316fbe6cf4c53a95bfa27c62ae5/18/jdk/buster/Dockerfile)
-	[`18.0.1.1-jdk-slim-buster`, `18.0.1.1-slim-buster`, `18.0.1-jdk-slim-buster`, `18.0.1-slim-buster`, `18.0-jdk-slim-buster`, `18.0-slim-buster`, `18-jdk-slim-buster`, `18-slim-buster`, `jdk-slim-buster`, `slim-buster`](https://github.com/docker-library/openjdk/blob/dd758df145819316fbe6cf4c53a95bfa27c62ae5/18/jdk/slim-buster/Dockerfile)
-	[`11.0.15-jdk-oraclelinux8`, `11.0.15-oraclelinux8`, `11.0-jdk-oraclelinux8`, `11.0-oraclelinux8`, `11-jdk-oraclelinux8`, `11-oraclelinux8`, `11.0.15-jdk-oracle`, `11.0.15-oracle`, `11.0-jdk-oracle`, `11.0-oracle`, `11-jdk-oracle`, `11-oracle`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jdk/oraclelinux8/Dockerfile)
-	[`11.0.15-jdk-oraclelinux7`, `11.0.15-oraclelinux7`, `11.0-jdk-oraclelinux7`, `11.0-oraclelinux7`, `11-jdk-oraclelinux7`, `11-oraclelinux7`](https://github.com/docker-library/openjdk/blob/77713ecc13f1480f3fe2b53fe03f2afb12727c74/11/jdk/oraclelinux7/Dockerfile)
-	[`11.0.15-jdk-bullseye`, `11.0.15-bullseye`, `11.0-jdk-bullseye`, `11.0-bullseye`, `11-jdk-bullseye`, `11-bullseye`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jdk/bullseye/Dockerfile)
-	[`11.0.15-jdk-slim-bullseye`, `11.0.15-slim-bullseye`, `11.0-jdk-slim-bullseye`, `11.0-slim-bullseye`, `11-jdk-slim-bullseye`, `11-slim-bullseye`, `11.0.15-jdk-slim`, `11.0.15-slim`, `11.0-jdk-slim`, `11.0-slim`, `11-jdk-slim`, `11-slim`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jdk/slim-bullseye/Dockerfile)
-	[`11.0.15-jdk-buster`, `11.0.15-buster`, `11.0-jdk-buster`, `11.0-buster`, `11-jdk-buster`, `11-buster`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jdk/buster/Dockerfile)
-	[`11.0.15-jdk-slim-buster`, `11.0.15-slim-buster`, `11.0-jdk-slim-buster`, `11.0-slim-buster`, `11-jdk-slim-buster`, `11-slim-buster`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jdk/slim-buster/Dockerfile)
-	[`11.0.15-jre-bullseye`, `11.0-jre-bullseye`, `11-jre-bullseye`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jre/bullseye/Dockerfile)
-	[`11.0.15-jre-slim-bullseye`, `11.0-jre-slim-bullseye`, `11-jre-slim-bullseye`, `11.0.15-jre-slim`, `11.0-jre-slim`, `11-jre-slim`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jre/slim-bullseye/Dockerfile)
-	[`11.0.15-jre-buster`, `11.0-jre-buster`, `11-jre-buster`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jre/buster/Dockerfile)
-	[`11.0.15-jre-slim-buster`, `11.0-jre-slim-buster`, `11-jre-slim-buster`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jre/slim-buster/Dockerfile)
-	[`8u332-jdk-oraclelinux8`, `8u332-oraclelinux8`, `8-jdk-oraclelinux8`, `8-oraclelinux8`, `8u332-jdk-oracle`, `8u332-oracle`, `8-jdk-oracle`, `8-oracle`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jdk/oraclelinux8/Dockerfile)
-	[`8u332-jdk-oraclelinux7`, `8u332-oraclelinux7`, `8-jdk-oraclelinux7`, `8-oraclelinux7`](https://github.com/docker-library/openjdk/blob/77713ecc13f1480f3fe2b53fe03f2afb12727c74/8/jdk/oraclelinux7/Dockerfile)
-	[`8u332-jdk-bullseye`, `8u332-bullseye`, `8-jdk-bullseye`, `8-bullseye`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jdk/bullseye/Dockerfile)
-	[`8u332-jdk-slim-bullseye`, `8u332-slim-bullseye`, `8-jdk-slim-bullseye`, `8-slim-bullseye`, `8u332-jdk-slim`, `8u332-slim`, `8-jdk-slim`, `8-slim`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jdk/slim-bullseye/Dockerfile)
-	[`8u332-jdk-buster`, `8u332-buster`, `8-jdk-buster`, `8-buster`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jdk/buster/Dockerfile)
-	[`8u332-jdk-slim-buster`, `8u332-slim-buster`, `8-jdk-slim-buster`, `8-slim-buster`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jdk/slim-buster/Dockerfile)
-	[`8u332-jre-bullseye`, `8-jre-bullseye`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jre/bullseye/Dockerfile)
-	[`8u332-jre-slim-bullseye`, `8-jre-slim-bullseye`, `8u332-jre-slim`, `8-jre-slim`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jre/slim-bullseye/Dockerfile)
-	[`8u332-jre-buster`, `8-jre-buster`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jre/buster/Dockerfile)
-	[`8u332-jre-slim-buster`, `8-jre-slim-buster`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jre/slim-buster/Dockerfile)

## Shared Tags

-	`20-ea-6-jdk`, `20-ea-6`, `20-ea-jdk`, `20-ea`, `20-jdk`, `20`:
	-	[`20-ea-6-jdk-oraclelinux8`](https://github.com/docker-library/openjdk/blob/7be88afe2fd7b6f4b28c7434a9c2d409c53fa0e3/20/jdk/oraclelinux8/Dockerfile)
-	`19-ea-31-jdk`, `19-ea-31`, `19-ea-jdk`, `19-ea`, `19-jdk`, `19`:
	-	[`19-ea-31-jdk-oraclelinux8`](https://github.com/docker-library/openjdk/blob/e3497a96e0b6c614bdd306d7d47ba32314545a48/19/jdk/oraclelinux8/Dockerfile)
-	`18.0.1.1-jdk`, `18.0.1.1`, `18.0.1-jdk`, `18.0.1`, `18.0-jdk`, `18.0`, `18-jdk`, `18`, `jdk`, `latest`:
	-	[`18.0.1.1-jdk-oraclelinux8`](https://github.com/docker-library/openjdk/blob/dd758df145819316fbe6cf4c53a95bfa27c62ae5/18/jdk/oraclelinux8/Dockerfile)
-	`11.0.15-jdk`, `11.0.15`, `11.0-jdk`, `11.0`, `11-jdk`, `11`:
	-	[`11.0.15-jdk-bullseye`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jdk/bullseye/Dockerfile)
-	`11.0.15-jre`, `11.0-jre`, `11-jre`:
	-	[`11.0.15-jre-bullseye`](https://github.com/docker-library/openjdk/blob/87352133c6e7e03310f992ca2827aa06df225f27/11/jre/bullseye/Dockerfile)
-	`8u332-jdk`, `8u332`, `8-jdk`, `8`:
	-	[`8u332-jdk-bullseye`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jdk/bullseye/Dockerfile)
-	`8u332-jre`, `8-jre`:
	-	[`8u332-jre-bullseye`](https://github.com/docker-library/openjdk/blob/da594d91b0364d5f1a32e0ce6b4d3fd8a9116844/8/jre/bullseye/Dockerfile)

[![arm64v8/openjdk build status badge](https://img.shields.io/jenkins/s/https/doi-janky.infosiftr.net/job/multiarch/job/arm64v8/job/openjdk.svg?label=arm64v8/openjdk%20%20build%20job)](https://doi-janky.infosiftr.net/job/multiarch/job/arm64v8/job/openjdk/)

# Quick reference (cont.)

-	**Where to file issues**:  
	[https://github.com/docker-library/openjdk/issues](https://github.com/docker-library/openjdk/issues)

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))  
	[`amd64`](https://hub.docker.com/r/amd64/openjdk/), [`arm64v8`](https://hub.docker.com/r/arm64v8/openjdk/), [`windows-amd64`](https://hub.docker.com/r/winamd64/openjdk/)

-	**Published image artifact details**:  
	[repo-info repo's `repos/openjdk/` directory](https://github.com/docker-library/repo-info/blob/master/repos/openjdk) ([history](https://github.com/docker-library/repo-info/commits/master/repos/openjdk))  
	(image metadata, transfer size, etc)

-	**Image updates**:  
	[official-images repo's `library/openjdk` label](https://github.com/docker-library/official-images/issues?q=label%3Alibrary%2Fopenjdk)  
	[official-images repo's `library/openjdk` file](https://github.com/docker-library/official-images/blob/master/library/openjdk) ([history](https://github.com/docker-library/official-images/commits/master/library/openjdk))

-	**Source of this description**:  
	[docs repo's `openjdk/` directory](https://github.com/docker-library/docs/tree/master/openjdk) ([history](https://github.com/docker-library/docs/commits/master/openjdk))

# What is OpenJDK?

OpenJDK (Open Java Development Kit) is a free and open source implementation of the Java Platform, Standard Edition (Java SE). OpenJDK is the official reference implementation of Java SE since version 7.

> [wikipedia.org/wiki/OpenJDK](http://en.wikipedia.org/wiki/OpenJDK)

Java is a registered trademark of Oracle and/or its affiliates.

![logo](https://raw.githubusercontent.com/docker-library/docs/a3439b66b7980d1811f6b3835a3c541747172970/openjdk/logo.png)

# How to use this image

## Start a Java instance in your app

The most straightforward way to use this image is to use a Java container as both the build and runtime environment. In your `Dockerfile`, writing something along the lines of the following will compile and run your project:

```dockerfile
FROM arm64v8/openjdk:11
COPY . /usr/src/myapp
WORKDIR /usr/src/myapp
RUN javac Main.java
CMD ["java", "Main"]
```

You can then run and build the Docker image:

```console
$ docker build -t my-java-app .
$ docker run -it --rm --name my-running-app my-java-app
```

## Compile your app inside the Docker container

There may be occasions where it is not appropriate to run your app inside a container. To compile, but not run your app inside the Docker instance, you can write something like:

```console
$ docker run --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp arm64v8/openjdk:11 javac Main.java
```

This will add your current directory as a volume to the container, set the working directory to the volume, and run the command `javac Main.java` which will tell Java to compile the code in `Main.java` and output the Java class file to `Main.class`.

## Make JVM respect CPU and RAM limits

On startup the JVM tries to detect the number of available CPU cores and RAM to adjust its internal parameters (like the number of garbage collector threads to spawn) accordingly. When the container is ran with limited CPU/RAM then the standard system API used by the JVM for probing it will return host-wide values. This can cause excessive CPU usage and memory allocation errors with older versions of the JVM.

Inside Linux containers, OpenJDK versions 8 and later can correctly detect the container-limited number of CPU cores and available RAM. For all currently supported OpenJDK versions this is turned on by default.

Inside Windows Server (non-Hyper-V) containers, the limit for the number of available CPU cores doesn't work (it's ignored by Host Compute Service). To set the limit manually the JVM can be started as:

```console
$ start /b /wait /affinity 0x3 path/to/java.exe ...
```

In this example CPU affinity hex mask `0x3` will limit the JVM to 2 CPU cores.

RAM limit is supported by Windows Server containers, but currently the JVM cannot detect it. To prevent excessive memory allocations, `-XX:MaxRAM=...` option must be specified with the value that is not bigger than the containers RAM limit.

## Environment variables with periods in their names

Some shells (notably, [the BusyBox `/bin/sh` included in Alpine Linux](https://github.com/docker-library/openjdk/issues/135)) do not support environment variables with periods in the names (which are technically not POSIX compliant), and thus *strip* them instead of passing them through (as Bash does). If your application requires environment variables of this form, either use `CMD ["java", ...]` directly (no shell), or (install and) use Bash explicitly instead of `/bin/sh`.

# Image Variants

The `arm64v8/openjdk` images come in many flavors, each designed for a specific use case.

## `arm64v8/openjdk:<version>`

This is the defacto image. If you are unsure about what your needs are, you probably want to use this one. It is designed to be used both as a throw away container (mount your source code and start the container to start your app), as well as the base to build other images off of.

Some of these tags may have names like bullseye or buster in them. These are the suite code names for releases of [Debian](https://wiki.debian.org/DebianReleases) and indicate which release the image is based on. If your image needs to install any additional packages beyond what comes with the image, you'll likely want to specify one of these explicitly to minimize breakage when there are new releases of Debian.

## `arm64v8/openjdk:<version>` (from 12 onwards), `arm64v8/openjdk:<version>-oracle` and `arm64v8/openjdk:<version>-oraclelinux8`

Starting with `openjdk:12` the default image as well as the `-oracle` and `-oraclelinux8` variants are based on the official [Oracle Linux 8 image](https://hub.docker.com/_/oraclelinux) which is provided under the GPLv2 as per the [Oracle Linux End User Agreement (EULA)](https://oss.oracle.com/ol8/EULA).

The `-oraclelinux7` variants are based on the official [Oracle Linux 7 image](https://hub.docker.com/_/oraclelinux) which is provided under the GPLv2 as per the [Oracle Linux End User Agreement (EULA)](https://oss.oracle.com/ol7/EULA).

The OpenJDK binaries are built by Oracle and are sourced from the [OpenJDK community](https://openjdk.java.net/). These binaries are licensed under the [GPLv2 with the Classpath Exception](https://openjdk.java.net/legal/gplv2+ce.html).

# License

View [license information](http://openjdk.java.net/legal/gplv2+ce.html) for the software contained in this image.

As with all Docker images, these likely also contain other software which may be under other licenses (such as Bash, etc from the base distribution, along with any direct or indirect dependencies of the primary software being contained).

Some additional license information which was able to be auto-detected might be found in [the `repo-info` repository's `openjdk/` directory](https://github.com/docker-library/repo-info/tree/master/repos/openjdk).

As for any pre-built image usage, it is the image user's responsibility to ensure that any use of this image complies with any relevant licenses for all software contained within.
