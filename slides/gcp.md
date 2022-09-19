## Network in GCP

----

### Cloud NAT

Cloud NAT lets certain resources without external IP addresses create outbound connections to the internet.
<img src="https://thecloudgirl.dev/images/CloudNAT.jpg" width="90%" />
Ref : https://thecloudgirl.dev/sketchnote.html

----

### Cloud NAT

Cloud NAT lets certain resources without external IP addresses create outbound connections to the internet.

<img src="img/cloud-nat.png" width="90%" />

----

### Cloud DNS

Cloud DNS is a high-performance, resilient, global Domain Name System (DNS) service that publishes your domain names to the global DNS in a cost-effective way

<img src="https://thecloudgirl.dev/images/CloudDNS.jpg" width="90%" />

----

### Cloud CDN

Cloud CDN enables customers to deliver content hosted on-premises or in another cloud over Google's high-performance distributed edge caching infrastructure

<img src="img/cloud-cdn.png" width="80%" />

----

### VPC

Virtual Private Cloud (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) clusters, and the App Engine flexible environment

VPC provides networking for your cloud-based resources and services that is global, scalable, and flexible

----

### VPC

<img src="img/vpc.png" width="75%" />

----

### Firewalls

VPC firewall rules let you allow or deny connections to or from your virtual machine (VM) instances based on a configuration that you specify.

Enabled VPC firewall rules are always enforced, protecting your instances regardless of their configuration and operating system, even if they have not started up.

----

### Routes

Google Cloud routes define the paths that network traffic takes from a virtual machine (VM) instance to other destinations. These destinations can be inside your Google Cloud Virtual Private Cloud (VPC) network (for example, in another VM) or outside it.

In a VPC network, a route consists of a single destination prefix in CIDR format and a single next hop. When an instance in a VPC network sends a packet, Google Cloud delivers the packet to the route's next hop if the packet's destination address is within the route's destination range.

----

### Cloud VPN (IPSec)

Cloud VPN securely connects your peer network to your Virtual Private Cloud (VPC) network through an IPsec VPN connection

Traffic traveling between the two networks is encrypted by one VPN gateway and then decrypted by the other VPN gateway

This action protects your data as it travels over the internet

----

### Cloud VPN (IPSec)

![Cloud VPN](img/cloud-vpn.png)

----

### Cloud Routers (BGP)

Cloud Router is a fully distributed and managed Google Cloud service that uses the Border Gateway Protocol (BGP) to advertise IP address ranges

![Cloud router](img/cloud-router.png)

----

### Interconnect

Cloud Interconnect provides low latency, high availability connections that enable you to reliably transfer data between your on-premises and Google Cloud Virtual Private Cloud (VPC) networks

Also, Interconnect connections provide internal IP address communication, which means internal IP addresses are directly accessible from both networks

----

### Interconnect

![Interconnect](img/interconnect.png)
