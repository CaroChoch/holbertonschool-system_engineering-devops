# Task 3: Scale up

Scaling up storage infrastructure aims to add resources supporting an application to improve or maintain ample performance. Both virtual and hardware resources can be scaled up. In the context of hardware, it may be as straightforward as using a larger hard drive to greatly increase storage capacity. Note, though, scaling up does not necessarily require changes to your system architecture.

Scaling up infrastructure is viable until individual components are impossible to scale anymore — making this a rather short-term solution.

![image](https://github.com/CaroChoch/holbertonschool-system_engineering-devops/assets/113856063/eb2b7a26-a993-4ee4-9771-154e54c3f393)

### Requirements

You must add:

- 1 server
- 1 load balancer (HAproxy) configured as a cluster with the other one
- Split components (web server, application server, database) with their own server

### Description of the Infrastructure

The infrastructure includes the following components:

1. Server
We add an additional server to enhance the reliability and performance of the infrastructure. With multiple servers, we can distribute the workload and provide redundancy, reducing the risk of a single point of failure.

2. Load Balancer (HAproxy)
The load balancer is added to distribute incoming requests across multiple servers. By configuring HAproxy as a cluster, we ensure high availability and improve the scalability of the infrastructure.

3. Split Components (Web Server, Application Server, Database)
We separate the components of the infrastructure onto their dedicated servers:
- `Web Server`: The web server is responsible for handling HTTP requests and serving static content, such as HTML, CSS, and images.
- `Application Server`: The application server executes the application logic, processes dynamic content, and generates responses to client requests.
- `Database`: The database server stores and manages the application's data.

### Specifics of the Infrastructure

- `Server`: The additional server enhances the infrastructure's reliability and fault tolerance by distributing the workload and providing redundancy. It allows for better resource utilization and improved performance.
- `Load Balancer (HAproxy)`: The load balancer evenly distributes incoming requests across multiple servers, improving scalability, performance, and availability. Configuring HAproxy as a cluster ensures that requests are handled by multiple load balancers, providing fault tolerance and load balancing capabilities.
- `Split Components`: Separating the web server, application server, and database onto their dedicated servers allows for better resource allocation, scalability, and flexibility. Each component can be optimized and scaled independently based on its specific requirements.
