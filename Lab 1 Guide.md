Lab 1: Router on a Stick
========================

### Purpose

### What You Will Need
>Note: Your pod diagram will help with deciding which routers and switch to used

1. 3 Routers
  1. One will be used for actual routing
  2. Two will be used as hosts
2. 1 Layer 2 Switch

### Diagram
Looking at your pod diagram and the diagram of the desired set up for this lab,
draw out a diagram with labels for all the **interfaces** you will use along
with the **hostnames** for each one of your devices.

Also consider how **subnets** (or **vlans**) will factor into your diagram.  You
will need to setup two subnets: 5 and 6. The networks are:

- Vlan 5: 192.168.5.0/24
- Vlan 6: 192.168.6.0/24

>If you are confused about how to design your diagram or about how subnetting
works, speak with your TA.  The internet also has a lot of resources on
subnetting.

### Important Terminology

- **switch**
- **router**
- **interface**
- **sub-interface**
- **hostname**: name of switch or router
    >en

    >conf t
    
    >hostname 'name'

- **subnet**
- **vlan**
- **trunking**
- **gateway**

### Completion Requirements
Make sure each host is able to ping itself, its gateway, and the other host.

### Host Configurations
As we do not have any actual PCs to configure, we must use routers to act as
hosts.  One router will represent a host on the vlan 5 network, while the other
will represent a host on the vlan 6 network.  Because the routers will be used
as hosts, they will need to be changed from a layer 3 device to a layer 2
device.  Do so on each router by the following:
    >no ip routing

Before setting up the ip addresses, make sure to configure the hostname for the
host of vlan 5 and vlan 6.

Next we need to setup a default gateway which will allow the host to leave its
local network or subnet.  For instance to setup the default gateway for vlan 5,
use the following command:
    >ip default gateway 192.168.5.1

Setup the vlan 6 host accordingly.

### Switch Configurations

### Router Configurations

### Verifying Connections
