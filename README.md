# Architecture
## Server:
Tomcat is an open-source Java Servlet Container and provides java HTTP web server environment in which java code can run. Therefore, clients will send their requests to Tomcat which is acted as the server and send back the responses. Tomcat is the component of a web server that interacts with java servlets. Tomcat mapping a URL to a particular servlet and ensuring that the URL requester has the correct access-right, usually including an IP address and port number of server.<br>
DHIS is an open source software platform for reporting, analysis and dissemination of data for all health programs. It’s actually a web application based on Java and dhis.war is a JAR file used to distribute a collection of JavaServer Pages, Java Servlets, XML files and other resources that together constitute a web application. This is why we choose to use tomcat,because tomcat is a server that can support java.<br>
## Client:
Client sends requests to server and receives responses from server. On a PC client, we can access to server using browser or similar applications that support HTTP protocol.
On a mobile client such as an android phone, you can access to server using some components that support HTTP protocol. Besides, there are many types of requests. For example, if you are collecting raw data in rural area, your mobile client will send a request sending data to DHIS database. You can also send request and receive the map of processed data in DHIS directly or send request to process data with methods you define in backend and receive the outcome of data in frontend. Because java is not very suitable for data processing, you may use Jpython or other programming language combined with Java when processing data in DHIS.<br>


# Description of Dhis2

DHIS2 is a tool for `collection`, `validation`, `analysis`, and `presentation` of aggregate and patientbased statistical data, tailored (but not limited) to integrated health information management activities<br>
It runs on any platform with a Java Runtime Environment (JRE 7 or higher) installed.<br>

# Installation of Dhis2
Installation

## installation for windows
You can find this method in Dhis2/Installation of Dhis2/windows.

## installation for Linux
You can find this method in Dhis2/Installation of Dhis2/Linux.
