<!--

********************************************************************************

WARNING:

    DO NOT EDIT "eclipse-temurin/README.md"

    IT IS AUTO-GENERATED

    (from the other files in "eclipse-temurin/" combined with a set of templates)

********************************************************************************

-->

**Note:** this is the "per-architecture" repository for the `i386` builds of [the `eclipse-temurin` official image](https://hub.docker.com/_/eclipse-temurin) -- for more information, see ["Architectures other than amd64?" in the official images documentation](https://github.com/docker-library/official-images#architectures-other-than-amd64) and ["An image's source changed in Git, now what?" in the official images FAQ](https://github.com/docker-library/faq#an-images-source-changed-in-git-now-what).

# Quick reference

-	**Maintained by**:  
	[Adoptium](https://github.com/adoptium/containers)

-	**Where to get help**:  
	[Adoptium Slack](https://adoptium.net/slack); [Adoptium Support](https://github.com/adoptium/adoptium-support/issues/new/choose)

# Supported tags and respective `Dockerfile` links

**WARNING:** THIS IMAGE *IS NOT SUPPORTED* ON THE `i386` ARCHITECTURE

[![i386/eclipse-temurin build status badge](https://img.shields.io/jenkins/s/https/doi-janky.infosiftr.net/job/multiarch/job/i386/job/eclipse-temurin.svg?label=i386/eclipse-temurin%20%20build%20job)](https://doi-janky.infosiftr.net/job/multiarch/job/i386/job/eclipse-temurin/)

# Quick reference (cont.)

-	**Where to file issues**:  
	[GitHub](https://github.com/adoptium/containers/issues); The [adoptium support](https://adoptium.net/support) page has more information on quality, roadmap and support levels for Eclipse Temurin builds. Vulnerabilities not related to Eclipse Temurin itself should be be raised to their respective projects (e.g Ubuntu vulnerabilities need to be raised directly to the Ubuntu project).

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))  
	[`amd64`](https://hub.docker.com/r/amd64/eclipse-temurin/), [`arm32v7`](https://hub.docker.com/r/arm32v7/eclipse-temurin/), [`arm64v8`](https://hub.docker.com/r/arm64v8/eclipse-temurin/), [`ppc64le`](https://hub.docker.com/r/ppc64le/eclipse-temurin/), [`s390x`](https://hub.docker.com/r/s390x/eclipse-temurin/), [`windows-amd64`](https://hub.docker.com/r/winamd64/eclipse-temurin/)

-	**Published image artifact details**:  
	[repo-info repo's `repos/eclipse-temurin/` directory](https://github.com/docker-library/repo-info/blob/master/repos/eclipse-temurin) ([history](https://github.com/docker-library/repo-info/commits/master/repos/eclipse-temurin))  
	(image metadata, transfer size, etc)

-	**Image updates**:  
	[official-images repo's `library/eclipse-temurin` label](https://github.com/docker-library/official-images/issues?q=label%3Alibrary%2Feclipse-temurin)  
	[official-images repo's `library/eclipse-temurin` file](https://github.com/docker-library/official-images/blob/master/library/eclipse-temurin) ([history](https://github.com/docker-library/official-images/commits/master/library/eclipse-temurin))

-	**Source of this description**:  
	[docs repo's `eclipse-temurin/` directory](https://github.com/docker-library/docs/tree/master/eclipse-temurin) ([history](https://github.com/docker-library/docs/commits/master/eclipse-temurin))

## Overview

The images in this repository contain OpenJDK binaries that are built by Eclipse Temurin.

# What is Eclipse Temurin ?

The Eclipse Temurin project provides code and processes that support the building of runtime binaries and associated technologies that are high performance, enterprise-caliber, cross-platform, open-source licensed, and Java SE TCK-tested for general use across the Java ecosystem.

![logo](https://raw.githubusercontent.com/docker-library/docs/cb27e17c8b50fddc58f1933d266a1a7686fea8ed/eclipse-temurin/logo.png)

# Do you provide JRE (Java Runtime Environment) Images?

JRE images for OpenJDK 8 and 11 are now available. OpenJDK 11+ JRE's can also be produced using `jlink` (see usage below).

# How to use this Image

To run a pre-built jar file with the latest OpenJDK 11, use the following Dockerfile:

```dockerfile
FROM i386/eclipse-temurin:11
RUN mkdir /opt/app
COPY japp.jar /opt/app
CMD ["java", "-jar", "/opt/app/japp.jar"]
```

You can build and run the Docker Image as shown in the following example:

```console
docker build -t japp .
docker run -it --rm japp
```

### Using a different base Image

If you are using a distribution that we don't provide an image for you can copy the JDK using a similar Dockerfile to the one below:

```dockerfile
# Example
FROM <base image>
ENV JAVA_HOME=/opt/java/openjdk
COPY --from=i386/eclipse-temurin:11 $JAVA_HOME $JAVA_HOME
ENV PATH="${JAVA_HOME}/bin:${PATH}"
```

### Creating a JRE using jlink

On OpenJDK 11+, a JRE can be generated using `jlink`, see the following Dockerfile:

```dockerfile
# Example of custom Java runtime using jlink in a multi-stage container build
FROM i386/eclipse-temurin:11 as jre-build

# Create a custom Java runtime
RUN $JAVA_HOME/bin/jlink \
         --add-modules java.base \
         --strip-debug \
         --no-man-pages \
         --no-header-files \
         --compress=2 \
         --output /javaruntime

# Define your base image
FROM debian:buster-slim
ENV JAVA_HOME=/opt/java/openjdk
ENV PATH "${JAVA_HOME}/bin:${PATH}"
COPY --from=jre-build /javaruntime $JAVA_HOME

# Continue with your application deployment
RUN mkdir /opt/app
COPY japp.jar /opt/app
CMD ["java", "-jar", "/opt/app/japp.jar"]
```

If you want to place the jar file on the host file system instead of inside the container, you can mount the host path onto the container by using the following commands:

```dockerfile
FROM i386/eclipse-temurin:11.0.12_7-jdk
CMD ["java", "-jar", "/opt/app/japp.jar"]
```

```console
docker build -t japp .
docker run -it -v /path/on/host/system/jars:/opt/app japp
```

# License

The Dockerfiles and associated scripts are licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).

Licenses for the products installed within the images:

-	OpenJDK: The project license is GNU GPL v2 with Classpath Exception.

As with all Docker images, these likely also contain other software which may be under other licenses (such as Bash, etc from the base distribution, along with any direct or indirect dependencies of the primary software being contained).

Some additional license information which was able to be auto-detected might be found in [the `repo-info` repository's `eclipse-temurin/` directory](https://github.com/docker-library/repo-info/tree/master/repos/eclipse-temurin).

As for any pre-built image usage, it is the image user's responsibility to ensure that any use of this image complies with any relevant licenses for all software contained within.
