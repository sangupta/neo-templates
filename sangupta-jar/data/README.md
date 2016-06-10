# ${projectName}

#if($badges)
#if($travisci)
[![Build Status](https://travis-ci.org/sangupta/${artifactID}.svg?branch=master)](https://travis-ci.org/sangupta/${artifactID})
#end
#if($coveralls)
[![Coverage Status](https://coveralls.io/repos/github/sangupta/${artifactID}/badge.svg?branch=master)](https://coveralls.io/github/sangupta/${artifactID}?branch=master)
#end
#if($sonatype)
[![Maven Version](https://maven-badges.herokuapp.com/maven-central/${groupID}/${artifactID}/badge.svg)](https://maven-badges.herokuapp.com/maven-central/${groupID}/${artifactID})
#end
#end

$description

#set($doubleHash = '##')
$doubleHash TODO

$doubleHash Usage

#if($sonatype)
$doubleHash Downloads

The latest released library can be downloaded from Maven Central using:

<dependency>
    <groupId>${groupID}</groupId>
    <artifactId>${artifactID}</artifactId>
</dependency>

The current development snapshot JAR can be obtained using JitPack.io as:

Add the following repository to Maven,

<repository>
    <id>jitpack.io</id>
    <url>https://jitpack.io</url>
</repository>

Then add the dependency as,

<dependency>
    <groupId>com.github.sangupta</groupId>
    <artifactId>${artifactID}</artifactId>
    <version>-SNAPSHOT</version>
</dependency>

#end

$doubleHash Versioning

For transparency and insight into our release cycle, and for striving to maintain backward compatibility, 
`${artifactID}` will be maintained under the Semantic Versioning guidelines as much as possible.

Releases will be numbered with the follow format:

```
<major>.<minor>.<patch>
```

And constructed with the following guidelines:

* Breaking backward compatibility bumps the major
* New additions without breaking backward compatibility bumps the minor
* Bug fixes and misc changes bump the patch

For more information on **SemVer**, please visit http://semver.org/.

#if($license)
$doubleHash License

```
 ${projectName}: ${description}
 Copyright (c) ${year}, Sandeep Gupta
 
 http://sangupta.com/projects/${artifactID}
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
```
#end
