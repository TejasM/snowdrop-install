Snowdrop Installer:

Purpose:

To enable ease of installation of the snowdrop module in the standalone version of JBOSS AS/EAP.

What-it-does:

It copies the necessary snowdrop and spring jars in their proper location within ${JBOSS_HOME}/modules.

It also modifies the standalone.xml and registers the snowdrop extension and subsystem, removing the need for manual tampering.

How-to-use:

NOTE: Make sure the environment variable JBOSS_HOME points to either your JBoss or EAP installation

Simply, run:

mvn package

By default snowdrop version 2.0.5.Final and spring 3.1.1.RELEASE will be installed. To change this simply execute:

mvn package -P${desired-spring-version} -Dversion.snowdrop=${desired-snowdrop-version}

There are four possible spring version profiles: spring-2.5, spring-3, spring-3.1 (the default), and spring-3.2.
