# Lab 03 — Isolated Host-Only Network

## Objective

Create an isolated network for cybersecurity experimentation so that vulnerable laboratory systems can communicate with each other without being directly exposed to the Internet.

## Network Architecture

The laboratory uses a dedicated VirtualBox Host-Only network:

```text
                 Internet
                    |
                 macOS Host
                    |
                  NAT
                    |
              10.0.2.0/24
                    |
               Kali Linux
                    |
        ------------------------
        |                      |
       eth0                   eth1
   10.0.2.15             192.168.56.2
                               |
                       Host-Only Network
                         192.168.56.0/24
                               |
                         macOS Host
                        192.168.56.1
