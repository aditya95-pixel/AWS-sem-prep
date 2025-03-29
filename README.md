# AWS-sem-prep

## Mod 2
## 1(a) What is Server Consolidation?

Server consolidation is the process of reducing the number of physical servers in an IT environment by using virtualization. Instead of running multiple applications on separate physical servers, virtualization allows multiple virtual machines (VMs) to run on a single physical machine. This optimizes resource utilization, reduces power consumption, lowers hardware costs, and simplifies management.

### Benefits of Server Consolidation:

Cost Savings: Fewer physical servers reduce hardware, maintenance, and power costs.

Efficient Resource Utilization: CPU, memory, and storage are better utilized.

Simplified Management: Centralized control and easier updates.

Scalability: Can easily scale workloads without adding new physical machines.


## 1(b) Distinguish Between Type I and Type II Hypervisors

### Type I Hypervisor (Bare-Metal Hypervisor)

Runs directly on the host machine's hardware.

Provides better performance and security.

Used in enterprise environments (e.g., VMware ESXi, Microsoft Hyper-V, Xen).

### Type II Hypervisor (Hosted Hypervisor)

Runs on top of a host operating system.

More suitable for personal use and testing environments.

Examples include VMware Workstation, VirtualBox, and Parallels.

### Schematic Diagram:

![alt text](https://github.com/aditya95-pixel/AWS-sem-prep/blob/main/type1type2hypervisor.png?raw=true)

## 1(c) Privileged and Non-Privileged Instructions

### Privileged Instructions

Can only be executed in kernel mode.

Directly interact with hardware (e.g., modifying control registers, I/O operations).

Example: Enabling/disabling interrupts.

### Non-Privileged Instructions

Can be executed in user mode.

Do not require direct access to hardware resources.

Example: Arithmetic and logical operations, reading the status of a register.

