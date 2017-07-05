## Introduction
DHIS2 is a open source software platform for collection, validation, analysis, and presentation of aggregate and patient-based statistical data, tailored to integrated health information management activities. [1] Techinically, DHIS2 is java-based web application and it follows a client-server architecture. In this document we will describe the architecture of DHIS, the different software components necessary to realize the function of this system and we will explain step-by-step how to install it in windows system or linux system.<br>
## Client–Server Architecture
The client–server architecture is a distributed application structure that partitions tasks or workloads between the providers of a resource or service, called servers, and service requesters, called clients.[2] Often clients and servers communicate over a computer network on separate hardware, but both client and server may reside in the same system. A server host runs one or more server programs which share their resources with clients. A client does not share any of its resources, but requests a server's content or service function. Clients therefore initiate communication sessions with servers which await incoming requests.As for web application such as DHIS2, client and server communicate following HTTP protocol. For more information about HTTP protocol, you can view the link https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol 
<br>
## Component -- Server:
As we mentioned, DHIS2 is a java-based web application installed on server. Therefore, we need to install Tomcat, which is an open-source Java Servlet Container and provides java HTTP web server environment in which java code can run. Specifically, Tomcat is the component of a web server that interacts with java servlets, mapping a URL to a particular servlet and ensuring that the URL requester has the correct access-right, usually including an IP address and port number of server.<br>
To install DHIS2 on Tomcat server, we need Ddhis.war file, a JAR file used to distribute a collection of JavaServer Pages, Java Servlets, XML files and other resources that together constitute a web application. Again, this is why we choose to use tomcat, because tomcat is a server that can support java.<br>
## Component -- Client:
There are several kinds of service requesters(clients) in our model. In a PC client, we can access to server using browser or similar applications that support HTTP protocol. In a mobile client such as an android phone, we can access to server using some android components that support HTTP protocol. Besides, there are many types of requests. For example, if you are collecting raw data in rural area, your mobile client will request to send data and store in DHIS database. You can also send requests for viewing the maps and figures the server already has. In another case, you request to process data in server with specific algorithms such as machine learning approach and receive the outcome in client. Because java is not very suitable for data processing, you may use Jpython or other programming language combined with Java when processing data in DHIS.<br>
<br>
The diagram below shows the component and functionality on server side and client side respectively and the communication model between server and client through request and response.
![image](https://github.com/zhangyuxuanProject/Dhis2/blob/master/Installation%20of%20Dhis2/Windows/Images/Architecture.png)<br>



## Installation Guide for Windows
You can find this method in Dhis2/Installation of Dhis2/windows.

## Installation Guide for Linux
You can find this method in Dhis2/Installation of Dhis2/Linux.

## Reference Webpages
[1] DHIS2 User Manual.Vers.2.27.Apr 2017 <http:www.dhis2.org><br>
[2] Client and server role <https://en.wikipedia.org/wiki/Client–server_model#Client_and_server_communication>
