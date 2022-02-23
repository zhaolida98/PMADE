#  Classifier Example

## Element details

## Project structure

This project is an example of element `classifier`.

There are 4 main modules, and each of them represent a possible value of element `classifier`. They are

| possible value | should be included in SCA BOM? |
| -------------- | ------------------------------ |
| client         | y                              |
| test           | n                              |
| javadoc        | n                              |
| source         | n                              |
| others         | y                              |

> Note that, although "source" is a valid option value, but no examples are found in all GitHub projects, thus, there is no example about "source"

## Operation

You can scan the project under the main folder `classifier` or go into sub-modules to scan one by one. Only results from `classifier-client` and `classifier-others` should be included. Ground truth are shown below

<details>
<summary>classifier-others</summary>
<pre>
com.sca.benchmark:classifier-others:jar:1.0-SNAPSHOT
\- net.sf.json-lib:json-lib:jar:jdk15:2.4:compile
 +- commons-beanutils:commons-beanutils:jar:1.8.0:compile
 +- commons-collections:commons-collections:jar:3.2.1:compile
 +- commons-lang:commons-lang:jar:2.5:compile
 +- commons-logging:commons-logging:jar:1.1.1:compile
 \- net.sf.ezmorph:ezmorph:jar:1.0.6:compile
</pre>
</details>

<details>
  <summary>classifier-client</summary>
  <pre>
com.sca.benchmark:classifier-client:jar:1.0-SNAPSHOT
\- org.jboss.jbossas:jboss-as-security:jar:client:5.1.0.CR1:compile
 +- javassist:javassist:jar:3.9.0.GA:compile
 +- org.jboss.security:jboss-security-spi:jar:2.0.3.SP1:compile
 +- org.jboss.security:jbosssx:jar:2.0.3.SP1:compile
 +- org.jboss:jboss-common-core:jar:2.2.13.GA:compile
 |  \- org.jboss.logging:jboss-logging-spi:jar:2.0.5.GA:compile
 +- org.jboss.jbossas:jboss-as-system-jmx:jar:5.1.0.CR1:compile
 |  +- apache-xerces:xml-apis:jar:2.9.1:compile
 |  +- org.jboss:jboss-vfs:jar:2.1.1.GA:compile
 |  +- org.jboss:jbossxb:jar:2.0.1.GA:compile
 |  |  +- org.jboss:jboss-reflect:jar:2.0.2.GA:compile
 |  |  +- wutka-dtdparser:dtdparser121:jar:1.2.1:compile
 |  |  +- javax.activation:activation:jar:1.1.1:compile
 |  |  \- sun-jaxb:jaxb-api:jar:2.1.9:compile
 |  +- org.jboss.deployers:jboss-deployers-core-spi:jar:2.0.6.GA:compile
 |  +- org.jboss.deployers:jboss-deployers-impl:jar:2.0.6.GA:compile
 |  |  +- org.jboss.deployers:jboss-deployers-spi:jar:2.0.6.GA:compile
 |  |  +- org.jboss.cl:jboss-classloading:jar:2.0.5.GA:compile
 |  |  |  \- org.jboss.cl:jboss-classloader:jar:2.0.5.GA:compile
 |  |  \- org.jboss:jboss-mdr:jar:2.0.1.GA:compile
 |  +- org.jboss.deployers:jboss-deployers-structure-spi:jar:2.0.6.GA:compile
 |  |  \- org.jboss.deployers:jboss-deployers-client-spi:jar:2.0.6.GA:compile
 |  +- org.jboss.deployers:jboss-deployers-vfs:jar:2.0.6.GA:compile
 |  |  +- org.jboss.cl:jboss-classloading-vfs:jar:2.0.5.GA:compile
 |  |  +- org.jboss.deployers:jboss-deployers-core:jar:2.0.6.GA:compile
 |  |  \- org.jboss.deployers:jboss-deployers-client:jar:2.0.6.GA:compile
 |  +- org.jboss.deployers:jboss-deployers-vfs-spi:jar:2.0.6.GA:compile
 |  |  \- stax:stax-api:jar:1.0:compile
 |  +- org.jboss.bootstrap:jboss-bootstrap:jar:1.0.0-Beta-3:compile
 |  |  \- org.jboss.man:jboss-managed:jar:2.0.0.GA:compile
 |  +- org.jboss.jbossas:jboss-as-system:jar:5.1.0.CR1:compile
 |  |  +- org.jboss.aop:jboss-aop:jar:2.1.0.CR3:compile
 |  |  |  +- org.apache.ant:ant:jar:1.7.0:compile
 |  |  |  |  \- org.apache.ant:ant-launcher:jar:1.7.0:compile
 |  |  |  +- qdox:qdox:jar:1.6.1:compile
 |  |  |  +- trove:trove:jar:2.1.1:compile
 |  |  |  +- log4j:log4j:jar:1.2.14:compile
 |  |  |  \- org.jboss.logging:jboss-logging-log4j:jar:2.0.5.GA:compile
 |  |  +- org.jboss.integration:jboss-profileservice-spi:jar:5.1.0.CR3:compile
 |  |  +- org.jboss.man:jboss-metatype:jar:2.1.0.CR8:compile
 |  |  \- org.jboss.microcontainer:jboss-aop-mc-int:jar:2.0.5.GA:compile
 |  +- org.jboss.jbossas:jboss-as-jmx:jar:5.1.0.CR1:compile
 |  |  +- org.jboss.jbossas:jboss-as-j2se:test-jar:tests:5.1.0.CR1:compile
 |  |  +- org.jboss.jbossas:jboss-as-mbeans:jar:5.1.0.CR1:compile
 |  |  |  +- dom4j:dom4j:jar:1.6.1:compile
 |  |  |  +- bcel:bcel:jar:5.1:compile
 |  |  |  |  \- regexp:regexp:jar:1.2:compile
 |  |  |  \- org.jboss.test:jboss-test:jar:1.1.4.GA:compile
 |  |  |     +- org.apache.ant:ant-junit:jar:1.7.0:compile
 |  |  |     +- jboss.profiler.jvmti:jboss-profiler-jvmti:jar:1.0.0.CR5:compile
 |  |  |     \- org.jboss.jbossas:jboss-server-manager:jar:1.0.2.GA:compile
 |  |  \- junit:junit:jar:3.8.2:compile
 |  +- org.jboss.microcontainer:jboss-dependency:jar:2.0.5.GA:compile
 |  \- org.jboss.microcontainer:jboss-kernel:jar:2.0.5.GA:compile
 +- org.jboss.javaee:jboss-ejb-api:jar:3.0.0.GA:compile
 |  +- org.jboss.javaee:jboss-transaction-api:jar:1.0.1.GA:compile
 |  \- org.jboss.ws.native:jbossws-native-jaxrpc:jar:3.0.4.GA:compile
 |     \- org.jboss.ws.native:jbossws-native-saaj:jar:3.0.4.GA:compile
 +- org.jboss.javaee:jboss-jacc-api:jar:1.1.0.GA_SP1:compile
 |  \- jboss.web:servlet-api:jar:2.1.1.GA:compile
 +- org.jboss.jbossas:jboss-as-j2se:jar:5.1.0.CR1:compile
 |  +- oswego-concurrent:concurrent:jar:1.3.4-jboss-update1:compile
 |  \- org.jboss.integration:jboss-classloading-spi:jar:5.1.0.CR3:compile
 +- org.jboss.naming:jnp-client:jar:5.0.1.GA:compile
 +- javax.security:jaas:jar:1.0.01:compile
 +- org.jboss.javaee:jboss-jaspi-api:jar:1.0.0.GA:compile
 +- org.jboss.security:jbosssx-client:jar:2.0.3.SP1:compile
 \- org.jboss.security:jbossxacml:jar:2.0.3:compile
  </pre>
</details>

  