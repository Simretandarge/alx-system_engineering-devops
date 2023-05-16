AOAAOAWhat happens when you type google.com in your browser and press Enter
•	In this article, we will go into the details of how these technologies work by tracing the steps from the moment you press the Enter button on your keyboard after typing https://www.google.com on the address bar of your browser till the Google search page we all know is displayed.
web page
A document that can be seen in a web browser, such as Firefox, Google Chrome, Opera, Microsoft Internet Explorer or Edge, or Apple's Safari, is known as a web page, however it is also sometimes referred to as just "pages."
Website
collection of related web sites that are typically connected in different ways. Commonly referred to as a "website" or "site."
Web server
A computer that hosts a website on the Internet.
DNS request
•	What is in a DNS request?
•	A DNS query (also known as a DNS request) is a demand for information sent from a user's computer (DNS client) to a DNS server. In most cases a DNS request is sent, to ask for the IP address associated with a domain name.

   TCP/IP
   TCP/IP stands for Transmission Control Protocol/Internet Protocol and is a suite of communication protocols. On the internet, network devices are connected using TCP/IP. An intranet or extranet is a type of private computer network that uses TCP/IP as its communication protocol.
  

   Firewall
    What does a computer firewall do?
    Internet traffic entering, leaving, or moving within a private network is restricted by a firewall, a computer network security device. By selectively      blocking or allowing data packets, this software, or dedicated hardware-software device, performs its purpose.

   HTTPS/SSL
     What is HTTPS and SSL?
      HTTPS uses an encryption protocol to encrypt communications. The protocol is called Transport Layer Security (TLS), although formerly it was           known as Secure Sockets Layer (SSL). This protocol secures communications by using what's known as an asymmetric public key infrastructure.

     Server
  .   What is a server?
•	A server can represent both hardware and software. When we are referring to hardware, especially the ones used by large companies like Google, we are talking about hundreds or even thousands of computers placed in large buildings called data centers, for the purpose of providing resources to clients based on requests. That being said any computer, including your laptop, can be used as a server if the appropriate server software is installed on it. Web servers, application servers, file servers, print servers and proxy servers are some examples of servers.
•	For the purpose of our discussion, we need to define what a web server and application server is. A web server is a piece of software that is designed to accept HTTP requests and serve static web pages, which are written in HTML, CSS or JavaScript. Nginx, Apache and Microsoft IIS are some of the most common web servers available.
•	But websites do a lot more than serving static pages. They interact with the user using their graphical user interface and also generate dynamic content based on behavior, user preferences and manipulate huge amounts of data stored in databases. Databases are organized collections of structured information designed to insert, delete, query, access and modify data efficiently.
•	Dynamic content is served using an application server. Application servers communicate with databases to manipulate data then generate static content from the dynamic content and send the data to web servers to send web pages to the clients.

Load balancers

An estimated 63,000 requests are handled by Google each second. They have thousands of strong servers operating round-the-clock to accomplish this. But it wouldn't be sufficient. They also need to figure out how to efficiently distribute requests to their servers. It seems sense that we don't want one server to handle ten requests while another is idle. Load balancers are useful in this situation.

To improve a system's availability, efficiency, and dependability, load balancers divide the workload. They could be software or hardware.
To fulfill their objectives, software load balancers employ one or more scheduling algorithms. Among the most popular algorithms are:
-Weighted scheduling distributes work to servers according to the weights given to each server. The hardware capabilities of each server are typically indicated by the weight. This technique is applied when there is a glaring gap between the servers' capabilities.
-Round Robin scheduling—suitable for servers with relatively equal capacities and less persistent connections—serves requests consecutively.
-When there is a lot of network traffic and the number of persistent connections between servers is not fairly distributed, the least connection first scheduling method—which priorities requests depending on which server has the fewest persistent connections—is highly helpful.

There are two types of hardware load balancers: layer 4 hardware load balancing, which use IP tunneling and DNS load balancing, and layer 7, which employs URL parsing, cookie sniffing, and HTTP reading.

Finally, these servers must use firewalls to filter out incoming and outgoing network traffic. Hardware or software security implementations known as firewalls permit, restrict, and block network traffic in accordance with a set of established rules. The Internet and a private network are typically placed between them.

Every full stack developer should be aware of the fundamental concepts of web infrastructure discussed in this article. I hope the reading was enjoyable.
   The  process
what happens when you type: https://www.google.com in your web browser	
	The browser goes to the DNS server and finds the real address (IP address) of the server that the website lives on.
	Once the IP address is known the browser makes an HTTP request (GET request) to the IP address to obtain the content of the site via the TCP/IP protocol.
	The request is checked by the server's firewall to make that everything is alright and there are not any security violations.
	Once the server (web server) receives the request sent by the browser after going through the firewall, the load balancer (server) if any, answers the request sending the data (also via TCP/IP protocol) along with the SSL certificate to initiate a secure session over HTTPS.
	Finally, the information is received by the web browser that made the request and now the information (usually: HTML, CSS, and JavaScript) is interpreted and rendered by the browser, showing the final result which is the website that you asked for, in this case: www.google.com
OOB
