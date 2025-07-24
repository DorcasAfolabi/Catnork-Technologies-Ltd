# Catnork-Technologies-Ltd
I designed a secure internal network for improved operational efficiency for catnork technologies ltd

# Project Overview
This project showcases a detailed functional internal network simulated for catnork technologies using cisco packect tracer featuring a routing protocol, switches, desktop PCs, a laptop used by an engineer, DHCP and DNS server and a web server hosting the internal company site. devices are grouped across departments and connected through different switches, with all traffic routed through a central router.After building the network with all necessary devices and services, Access Control List (ACL) was configured on the router to ensure that only the engineering laptop can access the webserver via HTTP. All other devices were restricted from HTTP access to the webserver but maintained access to other network services.

# Key features
# 1. Router: 
connects different networks such as LAN to the internet or to other LANs

# 2. Dynamic Host Configuration Protocol (DHCP): 
authomatically assigns IP addresses and other network settings to devices on a network

# 3. Domain Name System (DNS): 
this resolves domain name into IP addresses so that devices can locate and communicate with websites and services on the internet or internal networks.

# 3. Access Control List (ACLs):
this controls what traffic is allowed or denied on a network by matching specific conditions, helping to enforce security and traffic control.

# Devices and Configurations
## Key Devices
 # . Routers:
 Routes data and manage traffic between different networks 

 # . Switches:
   Connects devices within the same network

   # . Servers:
     Serve DHCP, DNS and Web application functions

   # . Endpoint Devices: 
     PCs and laptop

   # Configuration Steps

   # 1. Setup the Topology:
          . Arrange and connect router, switches and end devices 

   # 2. Configure Devices:
         . Assign static IP addresses to DHCP, DNS and web server, also create the gateway for each interface

  # 3. Configure DHCP Servers:
         . Define DHCP pools and scopes for each subnet.
         .  Bind interfaces to their respective pools.
         .  Enable DHCP server to assign IP addresses to end devices.
         
  # 4.  Apply ACLs:
         .  Define access rules to permit/deny traffic as required.
         .  Apply rules to the appropriate interfaces.

 # 5.   Test Connectivity:
         .  Test in browser:
 # Device     Action                     Result
 Laptop0      Visit http://192.168.2.4   Allowed
 Other PCs    Visit http://192.168.2.4   Blocked 
  

  
