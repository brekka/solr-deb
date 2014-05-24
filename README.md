Brekka Solr DEB
===============

Overview
--------

Repackages the standard Apache Solr zip distribution into a DEB archive for 
easy installation on Debian based Linux distributions. Currently this is very basic,
simply copying the files to the /usr/share/solr4 directory. You will need to setup
a web application container such as Jetty or Tomcat manually.


Releases
--------

The latest release is 4.8.1, and can be found here: [solr-deb-4.8.1.deb](https://brekka.org/maven/content/repositories/releases/org/brekka/solr-deb/4.8.1/solr-deb-4.8.1.deb)


Licence
-------

The Apache Software License, Version 2.0 - http://www.apache.org/licenses/LICENSE-2.0.html


Building
--------

The Apache Solr zip must be downloaded manually and placed in the local Maven 
repository under the following path:

    ${user}/.m2/repository/org/apache/solr/solr/[version]/solr-[version].zip

Once that is in place, the project can be built using Maven 3:

    mvn clean install
    

Usage
-----

##### Install using dpkg:

    dpkg -i solr_4.8.1_all.deb
    
The WAR file will be installed to: /usr/share/solr4/solr.war


