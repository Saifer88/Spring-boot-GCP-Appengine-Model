## How to use me

Fork the project, then install the [Google Cloud Platform SDK](https://cloud.google.com/sdk/)


Modify the pom to hook the GCP project here:

```xml
<configuration>
	<project>project-id</project>
	<version>${project.version}</version>
</configuration>
```

Then just compile & deploy with maven, using the plugin

```sh
$ mvn clean install
$ mvn appengine:deploy
```