---
title: "Type of Hypervisor6"
layout: single
collection: notes
category: "virtualization"
permalink: /notes/notes6
venue: "SAIT, ITS"
date: 2025-05-24
location: "Alberta, Canada"
---

Here's a simple explanation of the types of hypervisors

## The types of hypervisor

A hypervisor is software that allows you to create and run virtual machines (VMs). There are two main types:

### 1. Type 1 Hypervisor (also called Bare-metal Hypervisor)
It runs directly on the physical hardware (not on top of an operating system).

It's like the main controller of the computer.

Often used in data centers and by IT professionals.

Examples:

VMware ESXi

Microsoft Hyper-V (bare-metal version)

Xen

KVM (when used with Linux directly on hardware)

Proxmox VE (built on KVM)

🟢 Faster and more efficient because it talks directly to hardware.

### 2. Type 2 Hypervisor (also called Hosted Hypervisor)
It runs inside an existing operating system, like a normal application.

It uses the host OS to access hardware (slower than Type 1).

Best for personal computers and testing environments.

Examples:

VirtualBox

VMware Workstation / VMware Fusion

Parallels Desktop (for Mac)

🟡 Easier to set up, but slower because it runs on top of an OS.

🧠 Quick Summary Table
| Type   | Runs On              | Example Use Case       | Examples                       |
| ------ | -------------------- | ---------------------- | ------------------------------ |
| Type 1 | Directly on hardware | Servers, data centers  | ESXi, KVM, Proxmox             |
| Type 2 | On top of OS         | Home users, developers | VirtualBox, VMware Workstation |



