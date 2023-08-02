# 🧅 ESXi-Security-Onion-Passive Collection Platform 🧅

## Introduction

This showcases a project similar to what I have built and maintained in my professional work as a Junior Security Engineer while in the military. This cluster is meant to be used on a network as an additional security analysis tool for cyber threat hunting. 

This platform is based off ESXi hypervisors using several virtual machines of a Distributed Build of Security Onion version 2.3.100. 

A Security Onion Distributed Deployment contains the following:
- 1 Master/Manager Node
  - For a central management server in the distributed setup. Responsible for controlling activities of all other nodes in the deployment. 
- 1 Sensor/Forward Node (minimum)
  -  For capturing and processing network traffic and security events with Zeek/Suricata. 
- 1 Search Node (minimum)
  -  For storing and indexing the network logs generated by the Sensor Nodes.

Here is a picture showing the minimum build of a Security Onion Distributed Deployment from the [Security Onion Documentation Website](https://docs.securityonion.net/en/latest/architecture.html):

![image](https://github.com/gervguerrero/ESXi-Security-Onion-Passive-Collection-Platform-/assets/140366635/5cbc6295-e12d-4522-8653-ef46a7b6b2bd)

The highlight of a Distributed Builds allows for greater scalability and performance when adapting to different customer network sizes. Larger networks require more nodes to process a larger volume information, while smaller networks require less. Scaling up and down for Sensor/Forward and Search Nodes is as easy as plug and play to introduce your new asset to the Security Onion cluster, as long as they are built with the same Security Onion version. 

## Customized ESXi Security Onion Build 

![data collection platform purple](https://github.com/gervguerrero/ESXi-Security-Onion-Passive-Collection-Platform-/assets/140366635/fa6ad362-b50f-45a1-acc7-b10ea8f31acf)


