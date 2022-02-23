#  Profiles Example

## Element details

## Project structure

This project is an example of Maven project profiles.

There is only one module with two profiles, the default profile use `org.springframework.boot:spring-boot-starter-log4j2:2.6.1` as the dependency which use `org.apache.logging.log4j:log4j-api:2.14.1` as its transitive dependencies, while another profile specify the log4j versions to `2.17.1`. So, when scan in the "default" mode, it should only show `log4j` in `2.14.1`, but in "other" mode(trigger by `-Ddebug` when building), `log4j` should be in `2.17.1`. The tool should support getting different result from different profiles, or just combine them. 

## Operation

You should scan under the main module `profiles`. Ground truth are shown below

<details>
<summary>profiles-default</summary>
<pre>
 com.sca.benchmark:profiles:jar:1.0-SNAPSHOT
 \- org.springframework.boot:spring-boot-starter-log4j2:jar:2.6.1:compile
    +- org.apache.logging.log4j:log4j-slf4j-impl:jar:2.14.1:compile
    |  +- org.slf4j:slf4j-api:jar:1.7.25:compile
    |  \- org.apache.logging.log4j:log4j-api:jar:2.14.1:compile
    +- org.apache.logging.log4j:log4j-core:jar:2.14.1:compile
    +- org.apache.logging.log4j:log4j-jul:jar:2.14.1:compile
    \- org.slf4j:jul-to-slf4j:jar:1.7.32:compile
</pre>
</details>

<details>
<summary>profiles-other</summary>
<pre>
 com.sca.benchmark:profiles:jar:1.0-SNAPSHOT
 +- org.springframework.boot:spring-boot-starter-log4j2:jar:2.6.1:compile
 |  +- org.apache.logging.log4j:log4j-slf4j-impl:jar:2.14.1:compile
 |  |  \- org.slf4j:slf4j-api:jar:1.7.25:compile
 |  +- org.apache.logging.log4j:log4j-jul:jar:2.14.1:compile
 |  \- org.slf4j:jul-to-slf4j:jar:1.7.32:compile
 +- org.apache.logging.log4j:log4j-core:jar:2.17.1:compile
 \- org.apache.logging.log4j:log4j-api:jar:2.17.1:compile
</pre>
</details>

