#  Optional Example

## Element details

## Project structure

This project is an example of Maven project Optional.

There is only one module with only one dependency, `nacos-client` inside. Originally, this component has 19 direct dependencies, but 9 of them are optional, which means they will not be visible to the project who import it as a dependency, for example, `nacos-api`. However, `nacos-api` is packed as a shaded jar into the distribution package of `nacos-client` and it is actually used. This part should be counted.

## Operation

You should scan under the main module `optional`. Ground truth are shown below (TODO: examine the correctness)

<details>
<summary>Optional</summary>
<pre>
 com.alibaba.nacos:nacos-client:jar:2.1.0-SNAPSHOT
 +- org.slf4j:slf4j-api:jar:1.7.7:compile
 +- org.apache.logging.log4j:log4j-core:jar:2.13.3:compile
 +- org.apache.logging.log4j:log4j-api:jar:2.13.3:compile
 +- org.apache.logging.log4j:log4j-slf4j-impl:jar:2.13.3:compile
 +- com.alibaba.nacos:nacos-common:jar:2.1.0-SNAPSHOT:compile
 |  \- commons-io:commons-io:jar:2.7:compile
 +- com.alibaba.nacos:nacos-api:jar:2.1.0-SNAPSHOT:compile
 |  +- io.grpc:grpc-netty-shaded:jar:1.24.0:compile
 |  |  \- io.grpc:grpc-core:jar:1.24.0:compile
 |  |     +- com.google.code.gson:gson:jar:2.8.6:compile
 |  |     +- com.google.android:annotations:jar:4.1.1.4:compile
 |  |     +- io.perfmark:perfmark-api:jar:0.17.0:compile
 |  |     +- io.opencensus:opencensus-api:jar:0.21.0:compile
 |  |     \- io.opencensus:opencensus-contrib-grpc-metrics:jar:0.21.0:compile
 |  +- io.grpc:grpc-protobuf:jar:1.24.0:compile
 |  |  +- io.grpc:grpc-api:jar:1.24.0:compile
 |  |  |  +- io.grpc:grpc-context:jar:1.24.0:compile
 |  |  |  +- com.google.errorprone:error_prone_annotations:jar:2.3.2:compile
 |  |  |  \- org.codehaus.mojo:animal-sniffer-annotations:jar:1.17:compile
 |  |  \- io.grpc:grpc-protobuf-lite:jar:1.24.0:compile
 |  +- io.grpc:grpc-stub:jar:1.24.0:compile
 |  +- io.netty:netty-all:jar:4.1.59.Final:compile
 |  +- com.google.api.grpc:proto-google-common-protos:jar:1.17.0:compile
 |  +- com.google.protobuf:protobuf-java:jar:3.8.0:compile
 |  +- io.grpc:protoc-gen-grpc-java:pom:1.24.0:compile
 |  \- javax.annotation:javax.annotation-api:jar:1.3.2:compile
 +- ch.qos.logback:logback-classic:jar:1.2.3:compile
 +- ch.qos.logback:logback-core:jar:1.2.3:compile
 +- commons-codec:commons-codec:jar:1.11:compile
 +- com.fasterxml.jackson.core:jackson-core:jar:2.12.2:compile
 +- com.fasterxml.jackson.core:jackson-databind:jar:2.12.2:compile
 |  \- com.fasterxml.jackson.core:jackson-annotations:jar:2.12.2:compile
 +- org.apache.httpcomponents:httpasyncclient:jar:4.1.3:compile
 |  +- org.apache.httpcomponents:httpcore:jar:4.4.13:compile
 |  +- org.apache.httpcomponents:httpcore-nio:jar:4.4.13:compile
 |  +- org.apache.httpcomponents:httpclient:jar:4.5.12:compile
 |  \- commons-logging:commons-logging:jar:1.2:compile
 +- org.reflections:reflections:jar:0.9.11:compile
 |  +- com.google.guava:guava:jar:30.1-jre:compile
 |  |  +- com.google.guava:failureaccess:jar:1.0.1:compile
 |  |  +- com.google.guava:listenablefuture:jar:9999.0-empty-to-avoid-conflict-with-guava:compile
 |  |  +- com.google.code.findbugs:jsr305:jar:3.0.2:compile
 |  |  +- org.checkerframework:checker-qual:jar:3.5.0:compile
 |  |  \- com.google.j2objc:j2objc-annotations:jar:1.3:compile
 |  \- org.javassist:javassist:jar:3.21.0-GA:compile
 +- net.jcip:jcip-annotations:jar:1.0:compile
 +- io.prometheus:simpleclient:jar:0.5.0:compile
 +- org.yaml:snakeyaml:jar:1.23:compile
 +- junit:junit:jar:4.12:test
 |  \- org.hamcrest:hamcrest-core:jar:1.3:test
 +- org.mockito:mockito-core:jar:3.8.0:test
 |  +- net.bytebuddy:byte-buddy:jar:1.9.16:test
 |  +- net.bytebuddy:byte-buddy-agent:jar:1.9.16:test
 |  \- org.objenesis:objenesis:jar:3.1:test
 \- org.mockito:mockito-inline:jar:3.8.0:test
</pre>
</details>

