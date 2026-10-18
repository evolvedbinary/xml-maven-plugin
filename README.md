# XML Maven Plugin

[![Build Status](https://dl.circleci.com/status-badge/img/gh/evolvedbinary/xml-maven-plugin/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/evolvedbinary/xml-maven-plugin/tree/main)
[![Java 8](https://img.shields.io/badge/java-8-blue.svg)](https://adoptopenjdk.net/)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Maven Central](https://img.shields.io/maven-central/v/com.evolvedbinary.maven.mojohaus/xml-maven-plugin?logo=apachemaven&label=maven+central&color=green)](https://central.sonatype.com/search?namespace=com.evolvedbinary.maven.mojohaus)

## Provenance

This is a fork of the MojoHaus XML Maven Plugin from [mojohaus/xml-maven-plugin](https://github.com/mojohaus/xml-maven-plugin).

The purpose of our fork is to add further configuration options for the plugin.

## Support

Whilst this fork is an Open Source project, developing this plugin is not our key occupation. We are happy for users to open issues, however we make no claims that we will investigate or resolve them.

We will gladly accept and merge Pull-Requests that address issues, but they must be accompanied by tests and be compatible with Java 8+.

The original author of the plugin *may* also be able to offer you some support, see [mojohaus/xml-maven-plugin](https://github.com/mojohaus/xml-maven-plugin).

## Releasing

* Make sure `gpg-agent` is running.
* Execute `mvn -B release:prepare release:perform`

For publishing the site do the following:

```
cd target/checkout
mvn site
mvn scm-publish:publish-scm
```

See [AGENTS.md](AGENTS.md) for build, test and pull request conventions.
