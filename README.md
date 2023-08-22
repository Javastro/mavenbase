# mavenbase


[![mavenbase](https://img.shields.io/maven-central/v/org.javastro/javastro-mavenbase.svg?label=javastro-mavenbase)](https://search.maven.org/artifact/org.javastro/javastro-mavenbase/)

[![BOM](https://img.shields.io/maven-central/v/org.javastro/bom.svg?label=BOM)](https://search.maven.org/artifact/org.javastro/bom/)

Base maven POM for the maven builds in the javastro suite of software. Since version 0.4.0 this has been refactored to save out the BOM separately.

The  software  is deployed to the maven central 
repository using the [following instructions](http://central.sonatype.org/pages/apache-maven.html)
summarized below.
   
Check that the build and tests are passed

	mvn clean install

then deploy to the staging repository
   
	mvn deploy -P release

if this is successful then

	mvn nexus-staging:release -P release -pl base,bom

will release to the central repository


