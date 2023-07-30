### Notes

#### Environment
- Google's data centers were the first to achieve ISO 14001 certification, which is a standard that maps out a framework for an organization to enhance its environmental performance through improving resource efficiency and reducing waste.
- Google became the first major company to be carbon neutral.
- we were the first company to achieve 100% renewable energy.
- By 2030, we aim to be the first major company to operate completely carbon free.

#### Security
#### Hardware infra layer
##### Hardware design and provenance
- Both the server boards and the networking equipment in Google data centers are custom-designed by Google.
- Google also designs custom chips, including a hardware security chip that's currently being deployed on both servers and peripherals.
##### Secure boot stack
- Google server machines use a variety of technologies to ensure that they are booting the correct software stack, such as cryptographic signatures over the BIOS, bootloader, kernel, and base operating system image.
#####  Premises security 
- Incorporate multiple layers of physical security protections
#### Service deployment layer
##### Encryption of inter-service communication
- Google’s infrastructure provides cryptographic privacy and integrity for remote procedure call (“RPC”) data on the network.
- Google’s services communicate with each other using RPC calls.
- The infrastructure automatically encrypts all infrastructure RPC traffic that goes between data centers.
####  User identity layer
- Google’s central identity service, which usually manifests to end users as the Google login page, goes beyond asking for a simple username and password.
- The service also intelligently challenges users for additional information based on risk factors
- Users can also employ secondary factors
#### Storage services layer
-  Encryption at rest security feature and enables hardware encryption support in hard drives and SSDs.
####  Internet communication layer
- Google Front End, which ensures that all TLS connections are ended using a public-private key pair and an X.509 certificate from a Certified Authority (CA), as well as following best practices such as supporting perfect forward secrecy.
- The GFE additionally applies protections against Denial of Service attacks. Also provided is Denial of Service (“DoS”) protection
- Multi-tier, multi-layer DoS protections that further reduce the risk of any DoS impact on a service running behind a GFE.
#### Google's Operational security layer
- Intrusion detection - Rules and machine intelligence give Google’s operational security teams warnings of possible incidents.
- Reducing insider risk - Google aggressively limits and actively monitors the activities of employees who have been granted administrative access to the infrastructure
- Employee U2F use - To guard against phishing attacks against Google employees, employee accounts require use of U2F-compatible Security Keys.
- Software development practices - Google employs central source control and requires two-party review of new code. Google runs a Vulnerability Rewards Program where we pay anyone who is able to discover and inform us of bugs in our infrastructure or applications.
