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
### create database
DHIS is an open source software platform for reporting, analysis and dissemination of data for all health programs. Therefore we need to have the database to save, compute and analyze the data
Therefore, we recommend to install PostgreSQL(http://www.postgresql.org/download/windows/). 
The recommend version is `Postgresql9.6`.
### configure dhis2 file
After DHIS2 version 2.22 the configuration file is called dhis.conf and resides in the DHIS2 home folder given in the environmental variables. Create a folder `C:\DHIS2`. (https://drive.google.com/file/d/0B28a90FiUzeTWkllSlQ2a1U2bEE/view) to download the standard `dhis.conf` file and save it in the above folder. Make sure the configuration files details reflect the details of the database created. 
### Download Dhis2
Download the latest DHIS2 war file (https://www.dhis2.org/downloads) and copy it in to `webapps` folder 
of the Tomcat installation (i.e. C:\Program Files (x86)\Apache Software Foundation\Tomcat 8.5\webapps).
The lastest version 2.26 is our recommendation.
### Install Tomcat 8 "32-bit/64-bit Windows Service Installer"
`it is VERY important that you install only the service installer - not the 32 bit or 64bit windows zip`
The WAR file requires you to install a Java servlet container, this is why we choose to use tomcat,because tomcat is a server that can support java. Tomcat is the component of a web server that interacts with java servlets and map a URL to a particular servlet and ensuring that the URL requester has the correct access-right, usually including an IP address and port number of server.
(http://tomcat.apache.org/download-80.cgi) website is to download Tomcat.
The recommend version is Version 8.5.15.










