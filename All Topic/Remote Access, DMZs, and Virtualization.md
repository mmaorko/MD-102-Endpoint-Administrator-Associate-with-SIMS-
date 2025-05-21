
## 🔐 What is Remote Access?
Remote access refers to the ability to connect to a computer, network, or IT service from a remote location — meaning, you're not physically present at the site where the system or network is located.
## 🛠️ Common Remote Access Tools and Technologies:
| Technology                        | Description                                                                               |
| --------------------------------- | ----------------------------------------------------------------------------------------- |
| **VPN (Virtual Private Network)** | Encrypts internet traffic and securely connects a remote user to a private network.       |
| **RDP (Remote Desktop Protocol)** | Allows users to control a computer remotely using a graphical interface (mainly Windows). |
| **SSH (Secure Shell)**            | Provides secure command-line access to remote computers (mainly Linux/Unix).              |
| **TeamViewer / AnyDesk**          | Commercial tools for screen sharing and remote control of computers.                      |


## 🛡️ What is a DMZ (Demilitarized Zone)
A DMZ (Demilitarized Zone) is a secure buffer zone in a network that separates public-facing services from an organization’s internal/private network. It adds an extra layer of protection by isolating systems that interact with the outside world.

### DMZ Network Architecture:
          [Internet]
              |
          [Firewall 1]
              |
         --- [DMZ] ---
        |     Web,     |
        |   Mail, DNS  |
         --------------
              |
          [Firewall 2]
              |
      [Internal Network]



## 🖥️ What is Virtualization?
Virtualization is the process of creating a virtual (software-based) version of something instead of a physical one. It allows one physical machine to run multiple virtual machines (VMs), each with its own operating system and applications — all isolated from each other.

### 🧱 How It Works:
At the core of virtualization is a hypervisor — software that sits between the hardware and virtual machines.

[Physical Server]
      |
[Hypervisor (e.g., VMware, Hyper-V, KVM)]
      |
  +-----------+  +-----------+
  |  VM 1     |  |  VM 2     |
  | Linux     |  | Windows   |
  +-----------+  +-----------+

### 🧩 Types of Virtualization:
| Type                       | Description                                                                   |
| -------------------------- | ----------------------------------------------------------------------------- |
| **Server Virtualization**  | Run multiple server VMs on one physical server.                               |
| **Desktop Virtualization** | Access desktops remotely (VDI – Virtual Desktop Infrastructure).              |
| **Storage Virtualization** | Combine multiple physical storage devices into a single virtual storage pool. |
| **Network Virtualization** | Abstract physical network resources into logical segments (e.g., VLANs).      |

