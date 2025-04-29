# EIGRP Network Configuration

This repository contains the configuration for a network using EIGRP (Enhanced Interior Gateway Routing Protocol) to ensure full connectivity between all devices and access to the Khazar server.

## Network Overview

- **Routing Protocol**: EIGRP
- **IP Addressing**: 
  - Point-to-point links: `/30` subnets
  - Device networks: `/20` subnets
- **Key Requirements**:
  - All devices can ping each other
  - All devices can access the Khazar server
  - Maintained SSH connection

## Implementation Steps

1. **EIGRP Configuration**:
   - EIGRP was configured on all routers with the appropriate Autonomous System (AS) number
   - Network statements were added for all connected subnets
   - Auto-summary was disabled

2. **Interface Configuration**:
   - All router interfaces were configured with correct IP addresses
   - Appropriate subnet masks were applied (/30 for point-to-point, /20 for device networks)

3. **Connectivity Verification**:
   - Ping tests conducted between all devices
   - Traceroute tests performed to verify paths
   - Khazar server access tested from multiple devices
4. **Testing**:
   - Ping between PCs in different VLANs to confirm connectivity.
   - Ensure there is no packet loss.

## Project Files

- `.pkt` file containing the full Packet Tracer simulation.

