---
layout: post
title: "HPC Cluster Setup Part 1 - The Basics"
author: "Jacky Ko"
categories: journal
tags: [documentation,clusters,hpc,slurm]
image: 2019-09-12-Cluster-Setup-Part-1/slurm_overview.png
---

High performance computing (HPC) refers to the high speed calculations and data processing ability. A modern PC or even mobile devices could provide up to 5 billions calculations per CPU core per second, and a more powerful workstation could assemble more than 50 CPU cores and multiples GPU in a single chassis unit. However the computation power of a single PC is still limited, how could we boost up the calculation speed when we have multiple devices? The solution is the concept of HPC clusters.

## How Does HPC Cluster Work?
The HPC cluster is an assembly of one or more computational devices, which can be divided into three main components
- Nodes
- Network
- Storage

![alt text](./assets/img/2019-09-12-Cluster-Setup-Part-1/how-hpc-works.jpg "Main components of HPC cluster")



## References
[Building a Raspberry Pi Cluster](https://medium.com/@glmdev/building-a-raspberry-pi-cluster-784f0df9afbd)