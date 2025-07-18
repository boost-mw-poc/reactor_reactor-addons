# Reactor Addons

[![CI on GHA](https://github.com/reactor/reactor-addons/actions/workflows/publish.yml/badge.svg)](https://github.com/reactor/reactor-addons/actions/workflows/publish.yml)

[![Join the chat at https://gitter.im/reactor/reactor](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/reactor/reactor?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![Latest addons](https://maven-badges.herokuapp.com/maven-central/io.projectreactor.addons/reactor-extra/badge.svg?style=plastic)](https://mvnrepository.com/artifact/io.projectreactor.addons/reactor-extra)

# Addons List

# reactor-adapter

Bridge to RxJava 2 Observable, Completable, Flowable, Single, Maybe, Scheduler, and also SWT Scheduler, Akka Scheduler ...

# reactor-extra

Extra operations and processors for Reactor Core including mathematical operations to compute sum, average, min or max from numerical sources.

# Contributing an Add-on

### Build instructions

`Reactor` uses a Gradle-based build system. Building the code yourself should be a straightforward case of:

    git clone git@github.com:reactor/reactor-addons.git
    cd reactor-addons
    ./gradlew test

This should cause the submodules to be compiled and the tests to be run. To install these artifacts to your local Maven repo, use the handly Gradle Maven plugin:

    ./gradlew install

### Maven Artifacts

Snapshot and pre-release Maven artifacts are provided in the SpringSource snapshot repositories.
To add this repo to your Gradle build, specify the URL like the following:

    ext {
      reactorAddonsVersion = '3.6.0-RC3'
    }

    repositories {
      //maven { url 'https://repo.spring.io/snapshot' }
      mavenCentral()
    }

    dependencies {
      // Reactor Adapter (RxJava2, Akka Actors scheduler and more)
      compile "io.projectreactor.addons:reactor-adapter:$reactorAddonsVersion"
    }


## Documentation

* [Guides](https://projectreactor.io/docs) (Notably `reactor-core` reference guide which
contains a section [about testing](https://projectreactor.io/docs/core/release/reference/docs/index.html#testing))
* [Reactive Streams](https://www.reactive-streams.org/)

## Community / Support

* [GitHub Issues](https://github.com/reactor/reactor-addons/issues)

## License

Reactor is [Apache 2.0 licensed](https://www.apache.org/licenses/LICENSE-2.0.html).
