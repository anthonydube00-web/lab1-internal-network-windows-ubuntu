# lab1-internal-network-windows-ubuntu
Windows &amp; Ubuntu internal network configuration and connectivity test

# Lab 1 – Internal Network Configuration (Windows & Ubuntu)

## Objective
Configure a private internal network between a Windows 11 client and an Ubuntu server virtual machine and verify connectivity.

## Environment
- Host: macOS
- Hypervisor: UTM (QEMU ARM64)
- Windows VM: Windows 11 Pro
- Linux VM: Ubuntu Desktop
- Network Mode: Host-Only (Internal Network)

## Configuration
Both virtual machines were configured to use the same internal (host-only) network.

- Ubuntu IP: `192.168.128.2`
- Windows IP: `192.168.128.3`
- Subnet: `255.255.255.0`

## Verification

### Ubuntu Network Configuration
![Ubuntu ip a](ubuntu-ip-a.png)

### Windows Network Configuration
![Windows ipconfig](windows-ipconfig.png)

### Connectivity Test
The Windows client successfully pinged the Ubuntu server.

![Windows ping](windows-ping.png)

## Result
Successful internal network communication was established between Windows and Ubuntu using a host-only network. This confirms proper VM network isolation and configuration.

## Skills Demonstrated
- Virtual machine networking
- Host-only / internal network configuration
- Linux networking (`ip a`)
- Windows networking (`ipconfig`, `ping`)
- Troubleshooting VM connectivity
