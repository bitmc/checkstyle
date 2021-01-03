# Checkstyle

[![github actions](https://img.shields.io/badge/github_actions-checkstyle-brightgreen.svg)](https://github.com/bitmc/checkstyle/actions)
[![maven central](https://img.shields.io/badge/maven_central-checkstyle-blue.svg)](https://search.maven.org/artifact/com.github.bitmc/checkstyle)

* [Checkstyle](https://github.com/checkstyle/checkstyle) configuration for BITMC Java style

## Usage

### IDE

* Checkout the repository and import configuration into your IDE.
	```bash
	checkstyle/src/main/resources/com/github/bitmc/checkstyle/checks.xml
	```

### Maven

* Add a dependency in your POM.
	```xml
	<plugin>
		<groupId>org.apache.maven.plugins</groupId>
		<artifactId>maven-checkstyle-plugin</artifactId>
		<version>3.1.1</version>
		<configuration>
			<configLocation>com/github/bitmc/checkstyle/checks.xml</configLocation>
		</configuration>
		<dependencies>
			<dependency>
				<groupId>com.puppycrawl.tools</groupId>
				<artifactId>checkstyle</artifactId>
				<version>8.39</version>
			</dependency>
			<dependency>
				<groupId>com.github.bitmc</groupId>
				<artifactId>checkstyle</artifactId>
				<version>8.39.0</version>
			</dependency>
		</dependencies>
	</plugin>
	```

## License

* Apache License 2.0
