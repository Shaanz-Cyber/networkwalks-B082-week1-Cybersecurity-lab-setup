# Networkwalks-B082-week1-Cybersecurity-lab-setup
Building an isolated virtual lab for Pen Testing and Ethical Hacking

![Skill](https://img.shields.io/badge/Skill-Cybersecurity-red)
![OS](https://img.shields.io/badge/OS-Kali%20Linux-blue)
![Tools](https://img.shields.io/badge/Tool-VirtualBox-orange)

## Project Overview

The project focuses on setting up a virtual lab in VirtualBox in which Kali Linux would be used as an attacker VM to simulate real world attacks. This provides a controlled environment in which malware and custom exploits can be tested safely. This lab will be on an isolated virtual network, so later more VMs can be added to the same virtual network to ensure connectivity between all the VMs.

## Objectives

- Install and configure VirtualBox.
- Install/import Kali Linux as a VM.
- Create a private NAT Network for the lab.
- Assign that NAT Network to Kali VM as it's network.
- Verify Network Connectivity and DNS resolution.
- Taking a snapshot of the VM for recovery.
- Document the complete process.


## Purpose of the Lab

The lab will be used for cybersecurity learning and authorized security testing.
It can be used for activities like:
- Network Reconnaissance
- Port Scanning
- Vulnerability Assessment
- Packet Analysis
- Web Security Testing
- Exploitation Practice
- Security-tool Experimentation

# Lab setup Procedure

## Step-1 Install 7-zip

7-zip was installed to extract the Kali Linux vm-package, which was in .7z format.
### Tool: 7-zip


## Step-2 Install VirtualBox

VirtualBox was install as the Hypervisor

## Step-3 Create a NAT Network

A dedicated NAT Network was create in VirtualBox.
Configuration: Network Name
NATNetwork IPv4 Prefix: 10.0.0.0/24
DHCP: Enabled
IPv6: Disabled

A NAT Network creates an subnet where every future VM will be added so that they can be on the same network.

## Step-4 Install Kali Linux

The Kali Linux machine was extracted and imported into the Hypervisor.

## Step-5 Configure the Kali Linux Network

The network was configured and was assigned IP addresses that were within the NAT Network IP range.

## Step-6 Create a Clean Snapshot of the Kali Linux Instance

This snapshot save the state of the machine after it was freshly installed and will be used as a backdrop in case of the VM getting infected with malware etc.















