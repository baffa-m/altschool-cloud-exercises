## Subnet Information

- **Subnet Address:** 193.16.20.35/29

### Calculations:

1. **Network IP Address:**
   - The given IP address: 193.16.20.35
   - Subnet mask: /29 (which means 29 bits are used for network portion)
   - Therefore, to find the network address, we need to borrow 29 bits for the network portion.
   - Binary representation of the IP address: 11000001.00010000.00010100.00100011
   - The subnet mask in binary: 11111111.11111111.11111111.11111000
   - Applying bitwise AND operation:
     ```
     11000001.00010000.00010100.00100011 (IP address)
   & 11111111.11111111.11111111.11111000 (Subnet mask)
     -----------------------------------
     11000001.00010000.00010100.00100000 (Network address)
     ```
   - Converted back to decimal: 193.16.20.32
   - **Network IP Address:** 193.16.20.32

2. **Number of Hosts:**
   - Number of bits available for hosts = 32 (IPv4 address size) - 29 (bits used for network portion)
   - Therefore, 2^(32-29) - 2 = 2^3 - 2 = 8 - 2 = 6
   - **Number of Hosts:** 6

3. **Range of IP Addresses:**
   - The first IP address in the range is the network address + 1
     - 193.16.20.32 + 1 = 193.16.20.33
   - The last IP address in the range is the broadcast address - 1
     - 193.16.20.39 - 1 = 193.16.20.38
   - **Range of IP Addresses:** 193.16.20.33 to 193.16.20.38

4. **Broadcast IP Address:**
   - The broadcast address for a subnet is always the last address in the range.
   - **Broadcast IP Address:** 193.16.20.39
