# mavenbase

[![Build Status](https://travis-ci.org/javastro/mavenbase.svg?branch=master)](https://travis-ci.org/javastro/mavenbase)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/org.javastro/javastro-mavenbase/badge.svg)](https://maven-badges.herokuapp.com/maven-central/org.javastro/javastro-mavenbase/)


base maven POM for the maven builds in the javastro suite of software.

The  software  is deployed to the maven central 
repository using the [following instructions](http://central.sonatype.org/pages/apache-maven.html)
summarized below.
   
Check that the build and tests are passed

	mvn clean install

then deploy to the staging repository
   
	mvn deploy -P release

if this is successful then

	mvn nexus-staging:release -P release

will release to the central repository


