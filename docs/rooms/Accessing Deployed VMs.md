---
id: accessing-deployed-vms
title: Accessing Deployed VMs
sidebar_label: Accessing Deployed VMs
---

You have the ability to deploy virtual machines attached to particular rooms and tasks. These machines can only be accessed using a VPN connection. In this case, users need to download an OpenVPN configuration file from here. Once a user deploys a machine they will be given a internal IP address which they will be able to communicate with using the OpenVPN connection.

**Our OpenVPN configuration will only route users traffic if they're trying to access one of the machines on our network, all other traffic is routed through its own connection**. 

To reiterate, when a user is connected through our OpenVPN connection only traffic for 10.*.*.* networks are routed through the VPN.

**If you can't get a connection to a room working:**
Make sure you're connected to the VPN properly, and with just a single connection. Test using https://tryhackme.com/room/openvpn.

Remember - just because you can't navigate to it via your browser on the default HTTP port 80, doesn't mean the box is broken. This is where you have to enumerate! Not all machines run webservers at all. Equally, not all rooms have SSH servers. Always scan the machine first!

By default, Windows machines will not respond to ping.
