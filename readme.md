# Cyber Defense

This repository is for study and reference purposes for the Cyber Defence learning path on TryHackMe.

## Introduction

### Network Services

How to gain unauthorized access to a machine by exploiting network services.

SMB (Server Message Block Protocol) is a client-server communication protocol used for sharing access to files, printers, serial ports and other resources on a network.
SMB is a response-request protocol. Clients connect to servers using TCP/IP. Samba(open-source server) runs on Unix systems.

**Enumeration**:process of gathering info on a target in order to find potential attack vectors(causes) and aid in exploitation.Enumeration can be used to gather usernames, passwords, network information, hostnames, application data, services, or any other information that may be valuable to an attacker.

- SMB shared drives. Tool used is Enum4Linux for both Windows and Linux systems.

- 1st step: Port scanning using Nmap
- Find open ports and SMB

**Exploiting SMB**:Because we're trying to access an SMB share, we need a client to access resources on servers using SMBClient
syntax to remotely access SMB

```shell
smbclient //[IP]/[SHARE]
Followed by the tags:
-U [name] : to specify the user
-p [port] : to specify the port
```

remote acces when you have file containing service and key
ssh -i [your id_rsa file] username@<target IP>

## Threat and Vulnerability Management

## Security Operations & Monitoring

## Threat Emulation

## Incident Response and Forensics

## Malware Analysis
