# Project Requirements: Basic Network Design

## Objective
Design and configure a basic local area network (LAN) using Cisco Packet Tracer. The network will include a router, two switches, and four PCs. The goal is to establish a functioning network with proper IP addressing and connectivity.

## Network Topology
- **Router**: Connects to two switches.
- **Switches**: Each switch connects to two PCs.
- **PCs**: Four PCs distributed across the two switches.

## Devices and Configuration

### Router
- **Name**: Router1
- **Interfaces**:
  - **GigabitEthernet0/0**: Connects to Switch1.
  - **GigabitEthernet0/1**: Connects to Switch2.

### Switch1
- **Name**: Switch1
- **Ports Configuration**:
  - **FastEthernet0/1**: Connects to Router1 (GigabitEthernet0/0).
  - **FastEthernet0/2**: Connects to PC1.
  - **FastEthernet0/3**: Connects to PC2.
- **VLAN Configuration**:
  - **VLAN 10**: Used for the devices connected to Switch1.

### Switch2
- **Name**: Switch2
- **Ports Configuration**:
  - **FastEthernet0/1**: Connects to Router1 (GigabitEthernet0/1).
  - **FastEthernet0/2**: Connects to PC3.
  - **FastEthernet0/3**: Connects to PC4.
- **VLAN Configuration**:
  - **VLAN 20**: Used for the devices connected to Switch2.

### PC Configuration
- **PC1**:
  - **IP Address**: 192.168.1.10
  - **Subnet Mask**: 255.255.255.0
  - **Default Gateway**: 192.168.1.1
- **PC2**:
  - **IP Address**: 192.168.1.11
  - **Subnet Mask**: 255.255.255.0
  - **Default Gateway**: 192.168.1.1
- **PC3**:
  - **IP Address**: 192.168.2.10
  - **Subnet Mask**: 255.255.255.0
  - **Default Gateway**: 192.168.2.1
- **PC4**:
  - **IP Address**: 192.168.2.11
  - **Subnet Mask**: 255.255.255.0
  - **Default Gateway**: 192.168.2.1

## IP Addressing
- **Router Interface GigabitEthernet0/0**:
  - **IP Address**: 192.168.1.1
  - **Subnet Mask**: 255.255.255.0
- **Router Interface GigabitEthernet0/1**:
  - **IP Address**: 192.168.2.1
  - **Subnet Mask**: 255.255.255.0

## Configuration Tasks
1. **Router Configuration**:
   - Configure IP addresses on router interfaces.
   - Set up static routing or dynamic routing as required.

2. **Switch Configuration**:
   - Configure VLANs on each switch.
   - Assign switch ports to appropriate VLANs.
   - Set up trunking if necessary.

3. **PC Configuration**:
   - Assign static IP addresses, subnet masks, and default gateways to each PC.

4. **Connectivity Testing**:
   - Verify connectivity between PCs in the same VLAN.
   - Verify connectivity between PCs in different VLANs via the router.
   - Test connectivity to ensure proper routing.

## Deliverables
- **Cisco Packet Tracer File**: The .pkt file containing the network configuration.
- **Configuration Files**: Text files or screenshots of router and switch configurations.
- **Network Diagram**: A visual representation of the network topology.
- **IP Address Assignments**: A document listing the IP addresses assigned to each device.

## Additional Notes
- **Command Line Only**: Use only the command-line interface (CLI) for configuring the switches and router. Avoid using the graphical interface or automated configuration tools within Cisco Packet Tracer.
- **Documentation**: Ensure that all configurations are well-documented and clearly annotated in the configuration files.
- **Testing**: Perform thorough testing of the network to confirm that all devices can communicate as expected. Verify that the routing between VLANs is functioning correctly.
