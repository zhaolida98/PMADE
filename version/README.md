#  Version Example

## Element details

## Project structure

This project is an example of different version expressions.

There are 3 main modules, and each of them represent a possible version situation: version range, version in property, version in parent property.

## Operation

You can scan the project under the main folder `version` or go into sub-modules to scan one by one. Ground truth are shown below

`version-range`

```
com.sca.benchmark:version-range:jar:1.0-SNAPSHOT
\- junit:junit:jar:4.3.1:compile
```



`version-property`

```
com.sca.benchmark:version-property:jar:1.0-SNAPSHOT
\- junit:junit:jar:3.8.1:compile
```



`version-parent-property`

```
com.sca.benchmark:version-property:jar:1.0-SNAPSHOT
\- junit:junit:jar:3.8.1:compile
```

