#  Aggregate Example

## Element details

## Project structure

This project is an example of Maven project aggregation.

There are two modules: `aggrgate` and `aggregate_child1`. Where `aggregate_child1` is a submodule of `aggregate`.

No dependency is claimed by `aggregate`

`aggregate_child` has the following dependency tree:

```
com.sca.benchmark:aggregate-child1:jar:1.0-SNAPSHOT
 +- org.apache.logging.log4j:log4j-core:jar:2.14.1:compile
 \- org.apache.logging.log4j:log4j-api:jar:2.14.1:compile
```

## Operation

You should scan the project under folder `aggregate`. If the tool support aggregation, it will detect 2 components, otherwise, 0 dependency will be found.

ground truth list:

```
org.apache.logging.log4j:log4j-core:jar@2.14.1
org.apache.logging.log4j:log4j-api:jar@2.14.1
```