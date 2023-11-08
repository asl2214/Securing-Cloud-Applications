# Overview

![..](Images/Azure%20Cloud%20Security%20Network.png)

## Topology
The diagram's purpose is to show the flow of an Azure Cloud Security Network created from scratch on Microsoft Azure. To connect to the DVWA (D*am Vulnerable Web Application) containers, the network would first connect to the internet from the user's computer or device, then bypass through the security group firewall based on its rules set for inbound traffic of the virtual network with the subnet range of 10.0.0.0/16, and then bypass the load balancer. The load balancer would restrict access to the network when connecting to the jumpbox provisoner for access to the DVWA containers. A security firewall was set to allow specific inbound and outbound rules while load balancing ensured to maximize network capacity and high performance. The firewall would prevent unknown IP addresses from trying to access the web containers and the load balancer is used to prevent DDoS (Distributed Denial of Service) attacks and server failure. 

| Name	| Function |	IP Address	| Operating System |
| --- | --- | --- | --- |
|Jump Box |	Gateway |	10.0.0.4	| Linux | 
| Web-1 |	container |	10.0.0.5 |	Linux |
| Web-2 |	container |	10.0.0.6 |	Linux |
