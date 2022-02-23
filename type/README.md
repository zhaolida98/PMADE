#  Type Example

## Element details

## Project structure

This project is an example of element `type`.

There are 7 main modules, and each of them represent a possible value of element `type`. They are

| possible value | should be included in SCA BOM? |
| -------------- | ------------------------------ |
| jar            | y                              |
| test-jar       | n                              |
| ear            | y                              |
| ejb            | y                              |
| war            | y                              |
| rar            | y                              |
| pom            | y                              |
| javadoc        | n                              |

## Operation

You can scan the project under the main folder `type` or go into sub-modules to scan one by one. According to the table, only results from `type-jar`, `type-ear`, `type-ejb`, `type-war`, `type-rar` should should be included. Ground truth are shown below



`type-ejb`

```
com.sca.benchmark:type-ejb:pom:1.0-SNAPSHOT
\- org.jboss.weld.examples.jsf.translator:weld-jsf-translator-ejb:ejb:4.0.2.Final:compile
```



`type-war`

```
com.sca.benchmark:type-war:jar:1.0-SNAPSHOT
\- org.jboss.weld.examples.jsf.translator:weld-jsf-translator-war:war:4.0.2.Final:compile
```



`type-rar`

```
com.sca.benchmark:type-rar:jar:1.0-SNAPSHOT
\- org.tranql:tranql-connector-ra:rar:1.7:compile
```



`type-ear`

```
com.sca.benchmark:type-ear:jar:1.0-SNAPSHOT
\- org.jboss.weld.examples.jsf.translator:weld-jsf-translator-ear:ear:4.0.2.Final:compile
```



`type-pom`

```
com.sca.benchmark:type-pom:jar:1.0-SNAPSHOT
\- org.springframework:spring-web:pom:5.3.7:compile
   +- org.springframework:spring-beans:jar:5.3.7:compile
   \- org.springframework:spring-core:jar:5.3.7:compile
      \- org.springframework:spring-jcl:jar:5.3.7:compile
```



`type-jar`

```
com.sca.benchmark:type-jar:jar:1.0-SNAPSHOT
+- org.apache.logging.log4j:log4j-core:jar:2.17.1:compile
\- org.apache.logging.log4j:log4j-api:jar:2.17.1:compile
```

