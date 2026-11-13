# SOC Virtual Lab Setup

## 1. Lab Overview

A virtual lab was created using VMware Workstation to practice basic SOC operations and network communication between two different operating systems.

## 2. Lab Environment

| Component               | Configuration      |
| ----------------------- | ------------------ |
| Virtualization Platform | VMware Workstation |
| Machine 1               | windows pro        |
| Machine 2               | Ubuntu Server      |
| Network Mode            | NAT                |
| Network Type            | VMware NAT Network |

## 3. Virtual Machines

### Windows VM

- Operating System: Windows pro
- IP Address: `192.168.153.133`
- Network Mode: NAT
- Snapshot: Clean Snapshot Created

### Ubuntu Server VM

- Operating System: Ubuntu Server
- IP Address: `192.168.153.132`
- Network Mode: NAT
- Snapshot: Clean Snapshot Created

## 4. Network Connectivity

Both virtual machines were configured using VMware NAT networking.

The objective was to verify communication between Windows and Ubuntu Server.

### Windows to Ubuntu

Command:

```cmd
ping 192.168.153.132
```

Result:

- Packets Sent: 4
- Packets Received: 4
- Packets Lost: 0
- Packet Loss: 0%

Status: Successful

### Ubuntu to Windows

Command:

```bash
ping -c 4 192.168.153.133
```

Status: Successful

## 5. Network Diagram

```text
             VMware NAT Network
                192.168.153.0/24
                       |
              +--------+--------+
              |                 |
        Windows VM         Ubuntu Server
      192.168.153.133      192.168.153.132
              |                 |
              +------ Ping -----+
                 Connectivity
```

## 6. Snapshots

Clean snapshots were created for both virtual machines to provide a baseline state for future lab exercises.

- Windows: Clean Snapshot
- Ubuntu Server: Clean Snapshot

## 7. Screenshots

Screenshots documenting the virtual machines, network configuration, connectivity tests, and snapshots will be added here.

## 8. Key Learning Outcomes

- Created a virtual lab using VMware Workstation.
- Identified IP addresses using Windows and Linux commands.
- Used `ping` to test network connectivity.
- Understood basic ICMP Echo Request and Echo Reply communication.
- Verified connectivity between two virtual machines.

## 9. Conclusion

The virtual lab was successfully configured, and network connectivity between Windows and Ubuntu Server was verified using ICMP ping tests.

