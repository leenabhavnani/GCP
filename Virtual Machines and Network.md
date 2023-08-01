#### Notes

- A virtual private cloud, or VPC, is a secure, individual, private cloud-computing model hosted within a public cloud – like Google Cloud!
- Google VPC networks are global
- Resources can even be in different zones on the same subnet.
- With Compute Engine, users can create and run virtual machines on Google infrastructure.
- Compute Engine bills by the second with a one-minute minimum.
- **Sustained-use** discounts start to apply automatically to virtual machines the longer they run.
- **Committed-use discounts** A 57% discount off of normal prices in return for committing to a usage term of one year or three years.
- **Preemptible and Spot VMs**  Compute Engine has permission to terminate a job if its resources are needed elsewhere
- Preemptible VMs can only run for up to 24 hours at a time, but Spot VMs do not have a maximum runtime.
- **VPC routing tables** are built-in so you don’t have to provision or manage a router.
- They’re used to forward traffic from one instance to another within the same network, across subnetworks, or even between Google Cloud zones, without requiring an external IP address
- VPCs provide a global distributed firewall, which can be controlled to restrict access to instances through both incoming and outgoing traffic.
- Cloud Load Balancing provides cross-region load balancing, including automatic multi-region failover, which gently moves traffic in fractions if backends become unhealthy
- **Cloud DNS** is what translates internet hostnames to addresses.
- **Edge caching** refers to the use of caching servers to store content closer to end users

  ##### Google Virtual Private Clouds connection to other networks 
- Start with a Virtual Private Network connection over the internet and use the IPsec VPN protocol to create a “tunnel” connection
- To make the connection dynamic, a Google Cloud feature called Cloud Router can be used.
- Cloud Router lets other networks and Google VPC, exchange route information over the VPN using the **Border Gateway Protocol**.
- A second option is to consider “peering” with Google using Direct Peering.
- Peering means putting a router in the same public data center as a Google point of presence and using it to exchange traffic between networks.
- One downside of peering, though, is that it isn’t covered by a Google Service Level Agreement.
- Third option is Dedicated Interconnect. This option allows for one or more direct, private connections to Google.
- Fourth option is Partner Interconnect, which provides connectivity between an on-premises network and a VPC network through a supported service provider.
