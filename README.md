# Tycho Maven Parent POM
[![Build Status](https://travis-ci.org/lucacesari/tycho-maven-parent-pom.svg?branch=master)](https://travis-ci.org/lucacesari/tycho-maven-parent-pom)

A parent POM for Eclipse projects.

## How to use it?
First of all, add the parent configuration to your pom.
  ```
  <parent>
    <groupId>org.bewq</groupId>
    <artifactId>tycho-parent</artifactId>
    <version>0.0.1-SNAPSHOT</version>
  </parent>
  ```

Then, add the following repository configuration to your pom.
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

## License
This sofware is released under Eclipse Public Licese v1.0. See the LICENSE
file for more information.

