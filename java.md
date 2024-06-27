# Java etc

## Jar inspection
Show contents of jar manifest from cli: 
`unzip -q -c myarchive.jar META-INF/MANIFEST.MF`

## JDK versions
on MacOs: 
```
# show current:
/usr/libexec/java_home

# list all jdks:
/usr/libexec/java_home -V

# set jdk for current shell in bash/zsh
export JAVA_HOME="`/usr/libexec/java_home -v 1.8`"

# set jdk for fish shell

set -g -x JAVA_HOME (/usr/libexec/java_home -v 1.8)
```
