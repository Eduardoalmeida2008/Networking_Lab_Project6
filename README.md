# Networking_Lab_Project6
Advanced Networking Lab with 2 routers, 4 switches, 6 VLANs, and DHCP configuration. Demonstrates VLAN setup, trunking, inter-VLAN routing, DHCP relay, and connectivity testing.

# Networking Lab - Project 6

## Lab Overview
This lab demonstrates an advanced network setup using:
- 2 Routers (R1, R2)
- 4 Switches (Switch1, Switch2, Switch3, Switch4)
- 6 VLANs (VLAN10, VLAN20, VLAN30, VLAN40, VLAN50, VLAN60)
- DHCP configuration for all VLANs
- Inter-VLAN routing
- Connectivity testing with ping

## Objectives
- Configure VLANs on access switches
- Configure trunk ports to carry multiple VLANs
- Set up DHCP pools and assign IP addresses automatically
- Test connectivity between all VLANs
- Understand DHCP relay and centralized DHCP
- Document network configuration and results

## Topology
- Each access switch connects PCs in a "U" formation for clarity
- VLAN10–VLAN40 handled by R1 (centralized DHCP)
- VLAN50–VLAN60 handled by R2 (with DHCP relay when necessary)

## DHCP Configuration
- DHCP pools created for all VLANs
- DNS server configured as 8.8.8.8
- Subnetting correctly applied for each VLAN

## Prints / Documentation Order

### 1. VLAN Configuration
- `VLAN_Config_Switch1.png`
- `VLAN_Config_Switch2.png`
- `VLAN_Config_Switch3.png`
- `VLAN_Config_Switch4.png`

### 2. Router Configuration
- `R1_RunningConfig.png` (show running-config)
- `R2_RunningConfig.png` (show running-config)
- `R1_Subinterfaces.png`
- `R2_Subinterfaces.png`
- `R1_IPInterfaceBrief.png`
- `R2_IPInterfaceBrief.png`

### 3. DHCP Configuration
- `DHCP_VLAN10-40.png` (all VLANs from R1 in one print)
- `DHCP_VLAN50-60.png` (VLANs from R2 in one print)
- `PC_VLAN10.png`
- `PC_VLAN20.png`
- `PC_VLAN30.png`
- `PC_VLAN40.png`
- `PC_VLAN50.png`
- `PC_VLAN60.png`

### 4. Connectivity / Ping Tests
- `Ping_VLAN10_to_VLAN50.png`
- `Ping_VLAN20_to_VLAN40.png`
- `Ping_VLAN30_to_VLAN60.png`
- `Ping_VLAN50_to_VLAN10.png`
- `Ping_VLAN60_to_VLAN20.png`

## Notes
- This lab demonstrates a centralized DHCP setup with relay for VLANs on different routers.
- Each print documents the correct configuration and connectivity verification.
- Use this lab as a reference for advanced VLAN and DHCP setups in enterprise-style topologies.
