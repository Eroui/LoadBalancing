# LoadBalancing
Learning LoadBalancing and creating a load balancer from scratch.

## Table of content
- [Description](#description)
- [Prerequisites](#prerequisites)
    - [What is a workload?](#workload)
    - [What is load balancing?](#load_balancing)
        - [What is a load balancer?](#load_balancer)
    - [Round-Robin (RR)](#round_robin)
        - [Round Robin DNS](#round_robin_dns)

## Description <a name="description"></a> 
In this project, I'am going to try to learn the basics of load blancing, and try to make a load balancer from scratch.

During the learning/developement process, I'am going to include any usefull information in this Readme markdown file including any usefull source, and so this can serve as a set of flashback cards and why not help any other person interested to learn about the subject.

## Prerequisites <a name="prerequisites"></a>
Before to start lets take a look at some information, descriptions and definitions that might be required before starting to tackle main subject.

### What is a workload? <a name="workload"></a>
> In computing, **the workload** is the amount of processing that the computer has been given to do at a given time. The workload consists of some amount of application programming running in the computer and usually some number of users connected to and interacting with the computer's applications. Source: [https://searchdatacenter.techtarget.com/definition/workload]

#### An amount of labor
> **Workload** is the amount of work an individual has to do. There is a distinction between the actual amount of work and the individual's perception of the workload. Workload can also be classified as quantitative (the amount of work to be done) or qualitative (the difficulty of the work). Source: [https://en.wikipedia.org/wiki/Workload]

In general, we can think of a workload as a function or method to be executed in a computing resource.

### What is load balancing? <a name="load_balancing"></a>
> In computing, **load balancing** improves the distribution of workloads across multiple computing resources, such as computers, a computer cluster, network links, central processing units, or disk drives. Load balancing aims to optimize resource use, maximize throughput, minimize response time, and avoid overload of any single resource. Using multiple components with load balancing instead of a single component may increase reliability and availability through redundancy. Load balancing usually involves dedicated software or hardware, such as a multilayer switch or a Domain Name System server process. Source: [https://en.wikipedia.org/wiki/Load_balancing_(computing)]

#### What is a load balancer? <a name="load_balancer"></a>
> load balancer is a device [Or software ^_^] that distributes network or application traffic across a cluster of servers. Load balancing improves responsiveness and increases availability of applications. Source [https://www.citrix.com/glossary/load-balancing.html]

> A load balancer sits between the client and the server farm accepting incoming network and application traffic and distributing the traffic across multiple backend servers using various methods. By balancing application requests across multiple servers, a load balancer reduces individual server load and prevents any one application server from becoming a single point of failure, thus improving overall application availability and responsiveness. Source [https://www.citrix.com/glossary/load-balancing.html]
    
### Round-Robin (RR) <a name="round_robin"></a>
> **Round-Robin (RR)** is one of the algorithms employed by process and network schedulers in computing. As the term is generally used, time slices (also known as time quanta) are assigned to each process in equal portions and in circular order, handling all processes without priority (also known as cyclic executive). Round-robin scheduling is simple, easy to implement, and starvation-free. Round-robin scheduling can also be applied to other scheduling problems, such as data packet scheduling in computer networks. It is an operating system concept. Source: [https://en.wikipedia.org/wiki/Round-robin_scheduling]

I have already learned about RR in one of my academic courses (Also FIFO LIFO SJF...).
#### Round Robin DNS <a name="round_robin_dns"></a>
> **Round Robin DNS** is a technique of load distribution, load balancing, or fault-tolerance provisioning multiple, redundant Internet Protocol service hosts, e.g., Web server, FTP servers, by managing the Domain Name System's (DNS) responses to address requests from client computers according to an appropriate statistical model. Source [https://en.wikipedia.org/wiki/Round-robin_DNS]

> In its simplest implementation, Round-robin DNS works by responding to DNS requests not only with a single potential IP address, but with one out of a list of potential IP addresses corresponding to several servers that host identical services. The order in which IP addresses from the list are returned is the basis for the term round robin. With each DNS response, the IP address sequence in the list is permuted. Usually, basic IP clients attempt connections with the first address returned from a DNS query, so that on different connection attempts, clients would receive service from different providers, thus distributing the overall load among servers. Source [https://en.wikipedia.org/wiki/Round-robin_DNS]

