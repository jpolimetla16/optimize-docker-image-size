use jdeps to find dependencies from spring boot far jar.

jdeps --multi-release 17 --list-deps --ignore-missing-deps -cp BOOT-INF/lib/* BOOT-INF/classes  test-demo-0.0.1-SNAPSHOT.jar

java.base/jdk.internal.vm.annotation
   java.compiler
   java.desktop
   java.instrument
   java.logging
   java.management
   java.naming
   java.net.http
   java.prefs
   java.rmi
   java.scripting
   java.security.jgss
   java.sql
   java.sql.rowset
   java.transaction.xa
   java.xml
   jdk.jfr
   jdk.unsupported
   
   jdeps using comma seperated.
   jdeps --multi-release 17  --print-module-deps --ignore-missing-deps -cp BOOT-INF/lib/* BOOT-INF/classes  test-demo-0.0.1-SNAPSHOT.jar
   
   java.base,
   java.compiler,
   java.desktop,
   java.instrument,
   java.management,
   java.net.http,
   java.prefs,
   java.rmi,
   java.scripting,
   java.security.jgss,
   java.sql.rowset,
   jdk.jfr,jdk.unsupported
   
   