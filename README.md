,# Dhis2
Installation

## installation for windows
### JAVA installation
we need to install `JDK or JRE`(https://www.java.com/en/download/) because Dhis2 is a web application based on Java and dhis.war is a JAR file used to distribute a collection of JavaServer Pages, Java Servlets, XML files and other resources that together constitute a web application.
### set environment variables
The `environment variables` help the system find where the configuration files(java, dhis2) are
the following operations are: My Computer (Right Click) → Properties → Advanced system settings → Environmental Variables and then   Under “System Variables” click `New` to add following:
`Variable Name: DHIS2_HOME`<br>
`Value: C:\DHIS2`<br>
`Variable Name: JAVA_OPTS`<br>
`Value: -Xms512m -Xmx1024m -XX:PermSize=256m -XX:MaxPermSize=768m'`<br>
`Make sure `Path` variable include the path to JDK’s “bin” folders address (i.e. C:\Program Files (x86)\Java\jre1.8.0_101)`




