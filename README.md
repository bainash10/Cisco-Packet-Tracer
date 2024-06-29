# Cisco Packet Tracer


# Clear the concepts:

## Network Concepts

- **Network Address**: The first IP address in a subnet, representing the entire subnet.
- **Broadcast Address**: The last IP address in a subnet, used to send data to all devices on that subnet.
- **Subnet Mask**: A 32-bit number used in IPv4 networking to divide an IP address into two parts: the network address and the host address.
- **IP Address**: A unique numerical label assigned to each device connected to a computer network that uses the Internet Protocol for communication. It serves two main purposes: identifying the host or network interface and providing the location of the host in the network, enabling the routing of data packets between devices.
- **MAC Address**: Identifies a network interface card, used for local network communication, typically static, visible only within the local network.
- **Subnet**: A logically visible subdivision of an IP network. The practice of dividing a network into two or more networks is called subnetting.

## Network Classes

- **Class A**: IP Range 1.0.0.0 to 126.0.0.0, Default Subnet Mask 255.0.0.0.
- **Class B**: IP Range 128.0.0.0 to 191.255.0.0, Default Subnet Mask 255.255.0.0.
- **Class C**: IP Range 192.0.0.0 to 223.255.255.0, Default Subnet Mask 255.255.255.0.
- **Class D**: IP Range 224.0.0.0 to 239.255.255.255, Used for multicast.
- **Class E**: IP Range 240.0.0.0 to 255.255.255.255, Reserved for experimental use.

## Network Devices and Their Functions

#### Hub

- Operates at the Physical Layer (Layer 1).
- Used in Star Topology.
- Broadcasts data to all ports.
- Less intelligent, cheaper, and suitable for small networks.

#### Switch

- Operates at the Data Link Layer (Layer 2).
- Stores MAC addresses and uses them for efficient data transfer.
- Capable of broadcasting, multicasting, and unicasting.
- More efficient and secure than hubs, supports full-duplex mode.

#### Router

- Operates at the Network Layer (Layer 3).
- Connects different LANs and routes data between them.
- Stores routing tables and performs routing based on IP addresses.

#### Repeater

- Operates at the Physical Layer (Layer 1).
- Regenerates and amplifies signals to extend network reach.
- Simple two-port device with no configuration needed.

#### Gateway

- Operates at various layers, typically Network Layer (Layer 3) and above.
- Serves as a bridge between different networks that use different protocols and technologies.
- Translates and routes data from one network to another.
- Can also provide additional functionalities like firewall and security policies.

### Network Topologies

- **Bus Topology**: All devices are connected to a single central cable, known as the bus.
- **Star Topology**: Devices are connected to a central hub or switch.
- **Ring Topology**: Each device is connected to two other devices, forming a ring.
- **Mesh Topology**: Devices are interconnected, allowing multiple paths for data.
- **Hybrid Topology**: Combination of two or more different types of topologies.

## Command Line Interface (CLI) Commands

- **Ping**: Used to check the connectivity between devices.
- **ipconfig**: Displays network configuration details.
- **ipconfig /all**: Shows detailed network configuration including MAC addresses.
- **encapsulation**: Configures the type of encapsulation on an interface, such as PPP or Frame Relay.
- **nslookup**: Queries DNS servers to find IP addresses of domain names and vice versa.
- **tracert**: Traces the path that packets take from source to destination.
- **show run**: Displays the current configuration of the device.

## CLI Modes and How to Access Them

- **User EXEC Mode**: Basic monitoring commands.
  - **Access**: Enter the device CLI. You will be in User EXEC Mode by default.
  - **Prompt**: `Router>`
  
- **Privileged EXEC Mode**: Advanced commands and configurations.
  - **Access**: Type `enable` from User EXEC Mode.
  - **Prompt**: `Router#`
  
- **Global Configuration Mode**: System-wide configuration changes.
  - **Access**: Type `configure terminal` from Privileged EXEC Mode.
  - **Prompt**: `Router(config)#`
  
- **Interface Configuration Mode**: Configuration changes to specific interfaces.
  - **Access**: Type `interface [type] [number]` from Global Configuration Mode (e.g., `interface GigabitEthernet 0/0`).
  - **Prompt**: `Router(config-if)#`
  

# Overview of files

These files contains various network configurations and topologies implemented in Cisco Packet Tracer. The exercises performed include:

- **Practiced Topologies**: Understanding different network topologies and their setups.
- **Static Routing**: Configuring static routes to enable communication between different network segments.
- **Connecting Multiple Networks**: Establishing connections between multiple networks using routers and switches.
- **Functions of Network Devices**:
  - **Repeater**: Regenerating signals to extend network reach.
  - **Bridge**: Connecting different network segments.
  - **Switches**: Managing data traffic within a network using MAC address tables.
- **VLAN**: Creating and managing Virtual Local Area Networks for segmented network traffic.


## Configurations

### Static Routing

- Configured routers to enable static routing between different network segments.
- Assigned IP addresses to router interfaces and end devices.
- Defined gateways for devices to enable communication between different networks.

### VLAN Configuration

- Created VLANs to segment network traffic.
- Assigned specific ports to VLANs for better traffic management and security.



## Practice Examples

- **Connecting PCs**: Assigned IP addresses and subnet masks to PCs.
- **Using Switches and Routers**: Connected switches and routers to establish communication between different networks.
- **Static Routing with Two Routers**: Configured static routes between two routers to enable inter-network communication.

## Conclusion

These files demonstrates the setup and configuration of various network topologies and devices using Cisco Packet Tracer. The configurations performed are fundamental for understanding network design, management, and troubleshooting in real-world scenarios. 

Feel free to explore the provided Packet Tracer files and modify the configurations to suit different networking scenarios.
