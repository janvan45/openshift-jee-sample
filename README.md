openshift-jee-sample
====================

A sample app to be deployed on openshift environments

Note: to build this repository with maven you must specify "-Popenshift", eg "mvn clean package -Popenshift"

*dev*

* spring boot
    * mvn clean package -Psblocal
    * java -jar target\SampleApp-1.0.jar
    * (alt:) mvn spring-boot:run -Psblocal

* jetty+jndi+postgresql
    * mvn clean package
    * mvn jetty:run -Pjetty

* jetty+hsqldb
    * mvn clean package
    * mvn jetty:run -Pjetty_lo
