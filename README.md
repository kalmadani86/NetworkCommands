# NetworkCommands
NetworkCommandsAndTroubleShooting
#includes the commands for network troubleshooting and investigation 
[This will be a series of informative branches that will include not oly commands but also scripts for automation executes]

AWS Networking Components

Virtual Private Cloud (VPC)
Primary Network Interface , Elastic Network Interface (ENI) which is a virtual network interface card (NIC)
Security groups
Network Access List (NACL)
Subnets (private subnet and public subnets)
VPN connections
Internet Gateway
Network Address Translator (NAT) for private subnet to connect to the internet
Virtual Private Gateway (VPG) for private subnet to access the internet


VPN can be used to connect to external networks by:

AWS site to site VPN
AWS DirectConnect Plus VPN
AWS VPN CloudHub


For the protection of the VPC a layered security is neede and it is as follow:

Network Access List
Security Groups (can be applied accreoss multiple instances and can be added and modifiedafter an instance is created)
Host protection software
Routing tables


VPS Characterstics

- The network is defined between sub net ranges /16 - /28. i.e. x.x.x.x/n. The smaller n the larger host number we can have and the larger n we get less hosts

- VPC can be created using the CLI

- There are multiple ways to connect to VPC:

with external networks
with other VPCs
with subnets
with AWS servers


- To Create a network in AWS

STEP 1:Understanding the business needes:

Knowing the number of devices needing IP addresses
What goes into public and/or private subnet
How many Avalability zones are needed (2 Minimum)
Where would they be located (selecting the AZ)


STEP 2:

Select the IP addressing
Create the VPC
Create the subnet (private && || public)
Crreate the Gateway
assign security groups to the ssubnets
Create the routing tables for the public and privatesubnets
launch aninstance and choose where to locate it
