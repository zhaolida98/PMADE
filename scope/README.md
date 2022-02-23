#  Classifier Example

## Element details

## Project structure

This project is an example of element `scope`.

There are only one main module, and there are five direct dependencies in different scopes. They are

| possible value | should be included in SCA BOM? |
| -------------- | ------------------------------ |
| compile       | y                              |
| runtime       | y                              |
| provided      | n                              |
| test          | n                              |
| system        | y                              |


## Operation

You can scan the project under the main folder `scope` 

<details>
<summary>scope</summary>
<pre>
com.sca.benchmark:scope:jar:1.0-SNAPSHOT
+- org.springframework:spring-web:jar:5.3.7:compile
|  +- org.springframework:spring-beans:jar:5.3.7:compile
|  \- org.springframework:spring-core:jar:5.3.7:compile
|     \- org.springframework:spring-jcl:jar:5.3.7:compile
\- javax.servlet.jsp:jsp-api:jar:2.1:runtime
</pre>
</details>