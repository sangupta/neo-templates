# $projectName

This a content package project generated using the AEM Multimodule NEO template.

## Building

This project uses Maven for building. Common commands:

* From the root directory, run `mvn -PautoInstallPackage clean install` to build the bundle and content package and install to a CQ instance.

* From the bundle directory, run `mvn -PautoInstallBundle clean install` to build *just* the bundle and install to a CQ instance.

## Using with AEM Developer Tools for Eclipse

To use this project with the AEM Developer Tools for Eclipse:
* Import the generated Maven projects via the *Import:Maven:Existing Maven Projects* wizard
* Enable the Content Package facet on the `content` project by right-clicking on the project
* Select Configure, then Convert to Content Package... 
* In the resulting dialog, select `src/main/content` as the Content Sync Root.

## Using with VLT

To use vlt with this project, first build and install the package to your local CQ instance as described above. Then cd to `content/src/main/content/jcr_root` and run

```shell
$ vlt --credentials admin:admin checkout -f ../META-INF/vault/filter.xml --force http://localhost:4502/crx
```

Once the working copy is created, you can use the normal `vlt up` and `vlt ci` commands.

## Specifying CRX Host/Port

The CRX host and port can be specified on the command line with:

```shell
$ mvn -Dcrx.host=otherhost -Dcrx.port=5502 <goals>
```
