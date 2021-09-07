## Basics

----

### OSI Model

| Layer # | Name | Description |
|---|---|---|
| 7 | Application layer | Human-computer interaction layer, where applications can access the network services |
| 6 | Presentation layer | Ensures that data is in a usable format and is where data encryption occurs |
| 5 | Session layer | Maintains connections and is responsible for controlling ports and sessions |
| 4 | Transport layer | Transmits data using transmission protocols including TCP and UDP |
| 3 | Network layer | Decides which physical path the data will take |
| 2 | Data link layer | Defines the format of data on the network |
| 1 | Physical layer | Transmits raw bit stream over the physical medium |

----

### OSI Model

| Layer # | Name | Example protocols |
|---|---|---|
| 7 | Application layer | HTTP, FTP, DNS, SNMP |
| 6 | Presentation layer | SSL, TLS |
| 5 | Session layer | NetBIOS, PPTP |
| 4 | Transport layer | TCP, UDP |
| 3 | Network layer | IP, ARP, ICMP, IPSec |
| 2 | Data link layer | PPP, ATM, Ethernet |
| 1 | Physical layer | Ethernet, USB, Bluetooth, IEEE 802.11 |

----

### TCP/IP Model

| Layer # | Name | Example protocols |
|---|---|---|
| 4 | Application layer | HTTP, FTP, DNS, SNMP, SQL, SMB, SSL, TLS |
| 3 | Transport layer | TCP, UDP |
| 2 | Network layer | IP, ARP, ICMP, IPSec |
| 1 | Network interface layer | Ethernet, USB, Bluetooth, IEEE 802.11 |

----

### TCP

- TCP stands for Transmission Control Protocol
- TCP provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts communicating via an IP network
- TCP is connection-oriented, and a connection between client and server is established before data can be sent

----

### 3-way handshake

- 3 steps to initiate a connection
  - SYN (synchronized)
  - SYN/ACK (synchronize / acknowledge)
  - ACK (acknowleged)

![3-way handshake](img/syn-ack.png)

----

### UDP

- UDP stands for User Datagram Protocol
- Uses a simple connectionless communication model with a minimum of protocol mechanisms

----

### IPv4

- 32-bits address
- From 0.0.0.0 to 255.255.255.255
- Associated with a subnet mask to be able to identify a machine and the network associated with this machine
- For example
  - 192.168.0.1 is the IP address
  - 255.255.255.0 is the mask address

----

### Subnets

- Logical division of an IP network
- Routing prefix expressed in CIDR notation
- Followed by a / and ending with the bit-length of the prefix
- For example
  - 198.51.100.0/24
  - Addresses from 198.51.100.0 to 198.51.100.255 belongs to this network

----

### CIDR

Classless Inter-Domain Routing

- Class A : 10.0.0.0/8
  - 16 777 216 IPs available
- Class B : 172.16.0.0/16
  - 1 048 576 IPs available
- Class C : 192.168.0.0/24
  - 65 536 IPs available
- Class D : 224.0.0.0/32
  - Multicast
- Class E : 240.0.0.0/32
  - Reserved

----

### Ports

- A port is a communication endpoint
- A port number is always associated with an IP address of a host and the type of transport protocol used for communication (TCP or UDP)
- Specific port numbers are reserved to identify specific services
- Port numbers lower than 1024 identify the historically most commonly used services
- Higher-numbered ports are available for general use by applications

----

## Common port numbers

| Number | Assignment |
|---|---|
| 20 | File Transfer Protocol (FTP) Data Transfer |
| 21 | File Transfer Protocol (FTP) Command Control |
| 22 | Secure Shell (SSH) Secure Login |
| 25 | Simple Mail Transfer Protocol (SMTP) email delivery |
| 53 | Domain Name System (DNS) service |
| 80 | Hypertext Transfer Protocol (HTTP) used in the World Wide Web |
| 443 | HTTP Secure (HTTPS) HTTP over TLS/SSL |

----

### Firewalls

- A firewall is a network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules
- Operates on layer 4 of the OSI model
- Packet filter
  - The first reported type of network firewall is called a packet filter, which inspect packets transferred between computers. The firewall maintains an access control list which dictates what packets will be looked at and what action should be applied
- Connection tracking
  - Second-generation firewalls perform the work of their first-generation predecessors but also maintain knowledge of specific conversations between endpoints by remembering which port number the two IP addresses are using

![Firewall](img/firewall.png)

----

### DMZ

- A DMZ is a physical or logical subnetwork that contains and exposes an organization's external-facing services to an untrusted, usually larger, network such as the Internet
- Add an additional layer of security to an organization's local area network (LAN)

![Single FW](img/single-fw.png)
![Dual FW](img/dual-fw.png)

----

### DNS

- The **Domain Name System (DNS)** is a hierarchical and decentralized naming system for computers, services, or other resources connected to the Internet or a private network
- Associates various information with domain names assigned to each of the participating entities
- For example
  - A record : associate a DNS name to an IPv4
  - AAAA record : associate a DNS name to an IPv6
  - CNAME record : Alias of one name to another
  - NS record : Delegates a DNS zone to use the given authoritative name servers
  - MX record : Maps a domain name to a list of message transfer agents for that domain
  - SRV record

(For a complete list, please look here : https://en.wikipedia.org/wiki/List_of_DNS_record_types)

----

### NAT

- **Network address translation (NAT)** is a method of mapping an IP address space into another
- One Internet-routable IP address of a NAT gateway can be used for an entire private network

![NAT](img/nat.jpg)

----

### VPN / LS

----

### Router

----

### Routing (BGP)

----

### Static vs Dynamic (DHCP)