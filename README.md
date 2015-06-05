#shared-dictionaries
This repository contains only dictionaries that are not included in [GBIF parsers](https://github.com/gbif/parsers).
For all geography related files, this dictionary-based approach (hosted on GitHub) is a transition solution until we move to data provided by geonames.org.

## Maven
shared-dictionaries artifacts are deployed to [jCenter](https://bintray.com/winglongitude/maven/shared-dictionaries/view).
```
	<repositories>
    ...
		<repository>
			<id>jcenter</id>
			<url>http://jcenter.bintray.com/</url>
		</repository>
	</repositories>
  ...
	<dependency>
		<groupId>winglongitude</groupId>
		<artifactId>shared-dictionaries</artifactId>
		<version>${shared-dictionaries.version}</version>
	</dependency>
```

## Naming convention
 * [[ISO3166 2 letters country code]]_ISO3166-2.txt e.g. CA_ISO3166-2.txt
 * [[ISO3166 2 letters country code]]_StateProvinceName.txt e.g. CA_StateProvinceName.txt

## Assumptions
To simplify the usage of the dictionary files, we assume: 
 * Dictionaries files lookup ignores separators except space(s)
 * Dictionaries files lookup ignores accentuated character(s)
