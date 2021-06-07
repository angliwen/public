# Configuring Google Cloud HA VPN

## Overview
HA VPN is a high-availability (HA) Cloud VPN solution that lets you securely connect your on-premises network to your VPC network through an IPsec VPN connection in a single region. HA VPN provides an SLA of 99.99% service availability.

HA VPN is a regional per VPC, VPN solution. HA VPN gateways have two interfaces, each with its own public IP address. When you create an HA VPN gateway, two public IP addresses are automatically chosen from different address pools. When HA VPN is configured with two tunnels, Cloud VPN offers a 99.99% service availability uptime.

In this lab you create a global VPC called **vpc-demo**, with two custom subnets in **us-east1** and **us-central1**. In this VPC, you add a Compute Engine instance in each region. You then create a second VPC called **on-prem** to simulate a customer's on-premises data center. In this second VPC, you add a subnet in region **us-central1** and a Compute Engine instance running in this region. Finally, you add an HA VPN and a cloud router in each VPC and run two tunnels from each HA VPN gateway before testing the configuration to verify the 99.99% SLA.

## Objectives
In this lab, you learn how to perform the following tasks:
- Create two VPC networks and instances.
- Configure HA VPN gateways.
- Configure dynamic routing with VPN tunnels.
- Configure global dynamic routing mode.
- Verify and test HA VPN gateway configuration.

## Tasks
![Task Map](https://github.com/angliwen/public/blob/173539f65c16909c512fc62104e68ea35ecb7717/Configuring%20Google%20Cloud%20HA%20VPN/map.png)

## Review
In this lab you configured HA VPN gateways. You also configured dynamic routing with VPN tunnels and configured global dynamic routing mode. Finally you verified that HA VPN is configured and functioning correctly.

## Disclaimer
Lab instructions wholly provided by Google. \
Task mapping is my own work.
