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

### 2(a) What do you mean by Virtualization in Cloud Computing?
Virtualization in cloud computing refers to the creation of virtual instances of computing resources such as servers, storage, networks, and operating systems. It allows multiple virtual machines (VMs) to run on a single physical machine, optimizing resource utilization and scalability.

### 2(b) Virtualization Advantages and Disadvantages

**Advantages:**
- **Cost Efficiency:** Reduces the need for physical hardware, lowering operational expenses.
- **Scalability:** Resources can be easily allocated and adjusted as per demand.
- **Flexibility:** Virtual environments can be quickly created, modified, or deleted.

**Disadvantages:**
- **Performance Overhead:** Virtualization can introduce latency due to resource sharing.
- **Security Concerns:** Virtual machines share the same underlying hardware, increasing vulnerability to attacks.
- **Complexity:** Managing multiple virtualized environments can be challenging.

### 2(c) Full Virtualization
Full virtualization is a technique in which a virtual machine completely emulates the underlying hardware, allowing unmodified guest operating systems to run as if they were on a physical machine.

**Advantage:**
- Supports multiple operating systems without modification.

**Disadvantage:**
- Higher resource overhead due to full emulation of hardware.

### 2(d) Cloud Service Model for Virtual Machine Deployment
The described scenario falls under the **Infrastructure as a Service (IaaS)** model.

**Reason:**
- IaaS provides fundamental computing resources such as virtual machines, networking, and storage.
- Users have control over their virtual machines, including network configurations, operating system choices, and application installations.

### 3(a) Name Three Hardware Virtualization Techniques
1. **Full Virtualization:** Uses a hypervisor to create and manage virtual machines that fully emulate physical hardware.
2. **Para-Virtualization:** The guest operating system is modified to be aware of the virtualization environment, improving efficiency.
3. **Hardware-Assisted Virtualization:** Modern processors (e.g., Intel VT-x, AMD-V) provide dedicated instructions to support virtualization at the hardware level.

### 3(b) What is ISA, ABI, and API with Respect to a Machine Reference Model?
- **Instruction Set Architecture (ISA):** Defines the interface between software and hardware, specifying machine-level instructions.
- **Application Binary Interface (ABI):** Defines how applications interact with the operating system at the binary level (e.g., system calls, data types, conventions).
- **Application Programming Interface (API):** Provides a set of functions and protocols for software applications to communicate with an operating system or other software components.

### 3(c) Para-Virtualization
Para-virtualization is a virtualization technique where the guest operating system is modified to interact efficiently with the hypervisor, reducing overhead.

**Advantage:**
- Improved performance compared to full virtualization due to reduced emulation overhead.

**Disadvantage:**
- Requires modifications to the guest operating system, limiting compatibility.

### 3(d) Process-Level vs. System-Level Techniques in Execution Virtualization
- **Process-Level Virtualization:**
  - Virtualizes individual processes by providing an abstraction layer (e.g., Java Virtual Machine, Docker containers).
  - Allows execution of applications across different platforms without modification.

- **System-Level Virtualization:**
  - Virtualizes entire operating systems, allowing multiple OS instances to run on a single physical machine (e.g., VMware ESXi, KVM).
  - Provides complete isolation between virtual machines.

### 4(a) Security Rings and Privilege Modes of Instruction Execution
Security rings define different levels of privilege for executing instructions on a computer system. These privilege levels help maintain system security and stability by restricting direct access to critical system resources.

#### **Security Rings:**
1. **Ring 0 (Kernel Mode):**
   - Has full access to hardware resources.
   - Executes privileged instructions (e.g., memory management, I/O control).
   - Used by the operating system kernel.

2. **Ring 1 & Ring 2 (Device Drivers):**
   - Used by certain system services and device drivers that require higher privilege than user applications but less than the OS kernel.

3. **Ring 3 (User Mode):**
   - Executes non-privileged instructions.
   - Used by applications and software running on the OS.

#### **Schematic Diagram:**

![alt text](https://github.com/aditya95-pixel/AWS-sem-prep/blob/main/instructionmode.png?raw=true)

### 4(b) Components of a Virtualized Environment
1. **Guest:**
   - The virtual machine (VM) running within a virtualization environment.
   - It can be an operating system or an application running on virtualized resources.

2. **Host:**
   - The physical machine that provides hardware resources for virtualization.
   - It runs a hypervisor or virtualization software to manage virtual machines.

3. **Virtualization Layer:**
   - The layer responsible for abstracting and managing hardware resources.
   - Provides an interface between the host and guest.
   - Examples include hypervisors like VMware ESXi, KVM, and Microsoft Hyper-V.






