# Task 0: Simple web Stack. 

A simple web stack is the collection of software required for Web development.  

At a minimum, it contains an operating system (OS), a programming language, database software, and a Web server.  

LAMP is one commonly used Web stack.  

So, When the user types a URL and clicks enter/return, the browser makes an HTTP request to the server. Then the webserver process the HTTP request by responding back with HTML Contents.  

We will encounter the following concepts in a web infrastructure:  

### Server: 

A server is a computer or system that hosts and serves web applications and files. It is responsible for receiving and processing requests from clients, such as web browsers, and sending back the corresponding responses.

### Domain Name: 

A domain name is a human-readable address that is used to identify and access websites on the internet. It provides a user-friendly way to represent the IP address of the server hosting the website. It plays a crucial role in directing users to the correct server.

### DNS Record: 

The DNS (Domain Name System) record specifies how domain names are mapped to IP addresses. In the case of www.foobar.com, the DNS record for the "www" subdomain would typically be a CNAME (Canonical Name) record pointing to the main domain foobar.com or an A (Address) record specifying the IP address of the server.

### Web Server: 

The web server handles HTTP requests from clients and serves static files (such as HTML, CSS, JavaScript, and images) or routes dynamic requests to the appropriate application server. It manages the initial communication with the client, processes the request, and returns the response.

### Application Server: 

The application server hosts and executes the server-side code responsible for generating dynamic content and processing business logic. It interacts with the web server to receive requests, processes them, and generates the appropriate response, which is then sent back to the client.

### Database: 

The database is used to store and manage the application's data. It provides a structured way to organize, retrieve, and manipulate information. The application server communicates with the database to perform operations such as reading or writing data, running queries, and managing transactions.


### Communication with Users: 

The server communicates with the user's computer requesting the website using network protocols such as HTTP or HTTPS. The server receives the user's request, processes it, generates a response, and sends it back to the user's computer over the network.


## Potential Issues with this Infrastructure:

### SPOF (Single Point of Failure): 

If the entire infrastructure is hosted on a single server, it becomes a single point of failure. If the server fails or experiences issues, the website may become unavailable. To address this, redundancy and fault-tolerant measures like load balancing or server clustering can be implemented.

### Downtime during Maintenance: 

Performing maintenance or deploying new code often requires restarting the web server, resulting in a temporary downtime for the website. Mitigating strategies like using rolling deployments or utilizing multiple servers can help minimize the impact of downtime during maintenance.

### Limited Scalability: 

With a single server, it becomes challenging to handle a large volume of incoming traffic. Scaling options such as adding more servers, load balancing, or utilizing cloud infrastructure should be considered to accommodate increased traffic and ensure optimal performance.  


It's important to note that while this simple web stack can serve basic web applications, more complex and scalable infrastructures may involve additional components, caching layers, content delivery networks (CDNs), and other optimizations to address specific requirements.




![image](https://github.com/CaroChoch/holbertonschool-system_engineering-devops/assets/113856063/18902e0f-3563-4e9e-b7bb-dd0a7a3b7b5b)
