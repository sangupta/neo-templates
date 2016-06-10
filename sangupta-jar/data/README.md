# ${projectName}

#if($badges)
#if($travisci)
[![Build Status](https://travis-ci.org/sangupta/${artifactID}.svg?branch=master)](https://travis-ci.org/sangupta/${artifactID})
#end
#if($coveralls)
[![Coverage Status](https://coveralls.io/repos/github/sangupta/${artifactID}/badge.svg?branch=master)](https://coveralls.io/github/sangupta/${artifactID}?branch=master)
#end
#if($sonatype)
[![Maven Version](https://maven-badges.herokuapp.com/maven-central/com.sangupta/${artifactID}/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.sangupta/${artifactID})
#end
#end

$description

#set($doubleHash = '##')
$doubleHash TODO

$doubleHash Usage

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
