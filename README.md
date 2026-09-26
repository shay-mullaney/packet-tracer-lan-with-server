# Packet Tracer LAN with Web Server

## Project overview

This Cisco Packet Tracer project has three PCs and a web server connected to a switch on one local network. Server0 uses the IPv4 address `192.168.1.2`.

## What I configured

- Connected three PCs and Server0 to the switch
- Configured Server0 as a web server
- Enabled HTTP and HTTPS on Server0

## Testing

From PC0, I successfully pinged Server0 at `192.168.1.2`.

I then opened PC0's web browser and loaded the server's page using both `http://192.168.1.2` and `https://192.168.1.2`.

I also checked PC0's ARP table and found an entry matching Server0's IP address to its MAC address.

## What I learned

The IP address identifies the server PC0 wants to reach. Because both devices are on the same local network, PC0 sends an Ethernet frame addressed to Server0's MAC address, and the switch forwards it.

## Project file

Open `lan-with-server.pkt` in Cisco Packet Tracer to explore and test the network.
