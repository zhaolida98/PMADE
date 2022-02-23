#  Inheritance Example

## Element details

## Project structure

This project is an example of Maven project inheritance.

There are two modules. `inheritance` is the parents module, and `inheritance-child1` is the child module. Child module will inherit all  dependencies from parents module.

## Operation

You should scan under the child module `inheritance-child1`. Ground truth are shown below

<details>
<summary>Inheritance</summary>
<pre>
 com.sca.benchmark:inheritance-child1:jar:1.0-SNAPSHOT
 +- org.apache.logging.log4j:log4j-core:jar:2.17.1:compile
 +- org.apache.logging.log4j:log4j-api:jar:2.17.1:compile
 \- org.springframework.boot:spring-boot-starter-log4j2:jar:2.6.1:compile
    +- org.apache.logging.log4j:log4j-slf4j-impl:jar:2.14.1:compile
    |  \- org.slf4j:slf4j-api:jar:1.7.25:compile
    +- org.apache.logging.log4j:log4j-jul:jar:2.14.1:compile
    \- org.slf4j:jul-to-slf4j:jar:1.7.32:compile
</pre>
</details>

