# Network-Design
<h2>Scenario: </h2>
CETPA pharmaceutical company which is a subsidiary company of CETPA IT solutions is building a new pharmaceutical centre in Barwa commercial avenue, Doha, Qatar due to high demand for influenza treatment and testing. The centre includes modern equipped vaccination and testing labs. The new centre LAN (Local area Network) will incorporate 5 units: Head office (10 computer), packing and assembling (5 computers), sales (5computers), marketing (6computers), Influenza vaccination and testing lab (10 computers), 3 printers.

Building:03 floors, all computers and printers are on the ground floor apart from the IT labs- one lab located on the first floor and another located on the second floor.

You recently hired by Cetpa IT solutions. The project manager has asked you to help to plan and design the network infrastructure to meet the specific business requirement of new centre using packet tracer and or/ any software tool of your choice. The network Infrastructure should include switches, routers, wireless routers, cables, servers, printers and other network devices.

<h3>Network requirements: </h3>

-	36 computers 
-	3 printers 
-	Scalable network 
-	Reliable 
-	High traffic
  
Based on the topology analysis and the network requirements, a tree topology is used to design the CETPA network infrastructure. And that’s due to several reasons:

-	Tree topology offers scalability by allowing effortless addition of new nodes to the network as an organization grows. This makes it a great choice for accommodating network expansion as the organization expands in size.
-	The hierarchical structure of the tree topology ensures that if one node fails it won't affect the network. This provides a level of reliability, which is especially useful for maintaining network stability and uninterrupted operations.
-	The tree topology simplifies maintenance and fault identification making troubleshooting and addressing network performance issues more straightforward throughout the structure. This can lead to network management and reduced downtime.
-	Multiple hardware and software vendors support the tree topology ensuring integration with various network equipment and management tools.
-	The tree topology is renowned for its level of security making it well suited for environments where data security is a top priority, such as Wide Area Networks (WANs).

While there, are advantages to using the tree topology it's important to consider drawbacks. However, in instances the advantages of scalability, dependability and ease of upkeep render the tree topology an appealing option, for designing and managing networks.

Even though the installation is expensive, however, it is needed to bring to the company more competitive advantages. And as we have two IT labs building good network infrastructure is needed. 
<p align="center">
Tree Topology: <br/>
<img src="https://github.com/user-attachments/assets/e3e24be8-74f0-41ca-a4d4-bab03d24ec21" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />



<h2>Network design:</h2>
 
To design the network system, we have used the following:
<h4>Software used: </h4>
Cisco packet tracer. 
<h4>Topology: </h4> 
Tree topology. 
<h4>Hardware: </h4>
a. Host: <br/>
-	Ground floor: <br/>
3 printers are distributed in different places on the ground floor. <br/>
Marketing: 6 computers <br/>
Sales: 5 computers <br/>
Head office: 10 computers <br/>
Packing: 5 computers 
-	First floor: 5 computers
-	Second floor: 5 computers

b. Networking devices: 4 switches, 2 routers distributed as follows: 
-	Second floor: 1 switch 
-	First floor: 1 switch, 1 router
-	Ground floor: 2 switches, 1 router 

c.	Servers: DHCP server. 

Network scheme: 

192.168.1.X: second floor LAB 02

192.168.4.X: first floor LAB 01     

192.168.3.X: Router to Router Network (Between Floors) 

192.168.2.X:  Ground floor Marketing and sales 

192.168.5.X: Ground floor Head office and paking 

<h4>Configuration: </h4>

1. We have made use of the DHCP server within the router to assign dynamic IP addresses to the hosts.
  
To do that we have used the CLI to type these commands and we enabled the device's DHCP function. 

<p align="center">
DHCP Configuration: <br/>
<img src="https://github.com/user-attachments/assets/57e19f12-2959-40c7-a4da-afd126f69792" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
<img src="https://github.com/user-attachments/assets/52310563-68a9-482c-a2a4-ba4f0c070a23" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />

2. To enable connection between the LANs we have configured the router GigabitEthernet ports.
<p align="center">
LANs connection configuration: <br/>
<img src="https://github.com/user-attachments/assets/fd68f96f-d04b-41e8-94fd-9bfb514b1a9f" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
<img src="https://github.com/user-attachments/assets/ca01e210-e228-45ef-860d-3be984d385f3" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
<img src="https://github.com/user-attachments/assets/7455a27d-1c7f-4405-be18-7f3871d0d5fc" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />
   
3. To enable communication between different stages, the configuration was done using the RIP which a Routing information protocol:
<p align="center">
RIP configuration: <br/>
<img src="https://github.com/user-attachments/assets/eccc6a00-743c-4dee-8b16-c9c6702f76df" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
CEPTA network design: <br/>
<img src="https://github.com/user-attachments/assets/eccc6a00-743c-4dee-8b16-c9c6702f76df" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />

<h2>Testing: </h2>
   
After implementing the design and running it, we could successful results ensuring good connectivity and configuration. 
<p align="center">
First testing results of the network: <br/>
<img src="https://github.com/user-attachments/assets/f337b909-6b38-4f9f-885f-c249af7d28ef" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />
  
Testing the designed network:
The test has been conducted by sending a packet from source computer (department X) to destination computer (department Y). X and Y can be sales, marketing, head office, packing, lab 01 or lab 02. 
The packet can be in this form where you drag and drop it in the computer of the department source and drop again in the computer of the department destination. 


The testing can be also done through using the command line ping the destination IP address. 
<p align="center">
Sending packets to 192.168.1.5: <br/>
<img src="https://github.com/user-attachments/assets/1eb53510-a324-483c-a8f6-0a04fe572c21" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />

We have conducted the test in real time, but simulation mode can also be used. 
We first tested the routers then the connection between the different departments the following table present the results we have got. 

Company: CETPA IT Solutions <br />
Project name: Network Infrastructure of CETPA Pharmaceutical Barwa Center. <br />
Responsible: Network Engineer <br />
Date: 03/12/2023<br />
Purpose and scope of the project: Testing the designed network infrastructure of CETPA center. <br />
<br />
Test analysis: <br />
**Number of packets sent:** <br />
Overall: 178 packets<br />
Router 1: 1 (Router 2), 1 (Marketing), 1 (Head Office), 1 (Sales), 1 (Packing), 1 (Lab 01), 1 (Lab 02)<br />
Router 2: 1 (Router 1), 1 (Marketing), 1 (Head Office), 1 (Sales), 1 (Packing), 1 (Lab 01), 1 (Lab 02)<br />
Marketing department: 7 (Head Office), 3 (Sales), 6 (Packing), 3 (Lab 01), 7 (Lab 02)<br />
Sales department: 5 (Marketing), 2 (Head Office), 8 (Packing), 6 (Lab 01), 7 (Lab 02)<br />
Head office department: 4 (Marketing), 7 (Sales), 4 (Packing), 7 (Lab 01), 5 (Lab 02)<br />
Packing department: 5 (Marketing), 4 (Head Office), 8 (Sales), 3 (Lab 01), 6 (Lab 02)<br />
Lab 01: 3 (Sales), 6 (Marketing), 2 (Head Office), 8 (Packing), 7 (Lab 02)<br />
Lob 02:  7 (Marketing), 2 (Head Office), 5 (Packing), 2 (Lab 01), 5 (Sales)<br />

**Number of received successful packets:** <br />
Overall: 131 packets <br />
Router 1: 1 (Router 2), 1 (Marketing), 1 (Head Office), 1 (Sales), 1 (Packing), 1 (Lab 01), 1 (Lab 02)<br />
Router 2: 1 (Router 1), 1 (Marketing), 1 (Head Office), 1 (Sales), 1 (Packing), 1 (Lab 01), 1 (Lab 02) <br />
Marketing department: 5 (Sales), 2 (Head Office), 3 (Packing), 5 (Lab 01), 7 (Lab 02) <br />
Sales department: 2 (Marketing), 4 (Head Office), 4 (Packing), 2 (Lab 01), 5 (Lab 02) <br />
Head office department: 6 (Marketing), 2 (Sales), 3 (Packing), 2 (Lab 01), 3 (Lab 02)<br />
Packing department: 4 (Sales), 5 (Marketing), 2 (Head Office), 6 (Lab 01), 3 (Lab 02)<br />
Lab 01: 3 (Marketing), 6 (Head Office), 3 (Packing), 6 (Sales), 2 (Lab 02)<br />
Lob 02: 4 (Marketing), 3 (Head Office), 6 (Packing), 6 (Sales), 3 (Lab 01)<br />

**Number of failed packets:** <br />
Overall: 47 <br />
Router 1: 0 (Router 2), 0 (Marketing), 0 (Head Office), 0 (Sales), 0 (Packing), 0 (Lab 01), 0 (Lab 02)<br />
Router 2: 0 (Router 1), 0 (Marketing), 0 (Head Office), 0 (Sales), 0 (Packing), 0 (Lab 01), 0 (Lab 02) <br />
Marketing department: 0 (Sales), 2 (Head Office), 2 (Packing), 1 (Lab 01), 0 (Lab 02) <br />
Sales department: 1 (Marketing), 3 (Head Office), 4 (Packing), 1 (Lab 01), 0 (Lab 02) <br />
Head office department: 1 (Marketing), 0 (Sales), 5 (Packing), 1 (Lab 01), 2 (Lab 02) <br />
Packing department: 4 (Sales), 1 (Marketing), 2 (Head Office), 2 (Lab 01), 2 (Lab 02) <br />
Lab 01: 0 (Sales), 0 (Marketing), 1 (Head Office), 0 (Packing), 0 (Lab 02) <br />
Lob 02: 3 (Marketing), 1(Sales), 2 (Head Office), 2 (Packing), 4 (Lab 01)<br />
