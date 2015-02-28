# Tycho Maven Parent POM
[![Build Status][travis-image]][travis-url]
[![EPL License][license-image]][license-url]

A parent POM for Tycho projects.

## How to use it?
First of all, add the parent configuration to your pom.
  ```
  <parent>
    <groupId>org.bewq</groupId>
    <artifactId>tycho-parent</artifactId>
    <version>0.0.1-SNAPSHOT</version>
  </parent>
  ```

Add the following repository configuration to your pom.
  ```
  <repositories>
    ...
    <repository>
      <id>tycho-maven-parent-pom-release</id>
      <name>Tycho Maven Parent POM Release</name>
      <releases>
        <enabled>false</enabled>
      </releases>
      <snapshots>
      <enabled>true</enabled>
      </snapshots>
      <url>https://raw.github.com/lucacesari/tycho-maven-parent-pom.git/snapshot</url>
    </repository>
  </repositories>
  ```

As final step, add a property named **tycho.scmUrl** and set your git
repository URL as its value.
  ```
  <properties>
    ...
    <tycho.scmUrl>scm:git:https://github.com/user.name/repository.git</tycho.scmUrl>
    ....
  </properties
  ```
## License
This software is released under Eclipse Public License v1.0. See the LICENSE
file for more information.

[travis-url]:https://travis-ci.org/lucacesari/tycho-maven-parent-pom
[travis-image]:https://img.shields.io/travis/lucacesari/tycho-maven-parent-pom.svg?style=flat-square

[license-url]:LICENSE
[license-image]:https://img.shields.io/badge/license-EPL-blue.svg?style=flat-square

