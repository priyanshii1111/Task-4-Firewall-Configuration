# Task-4-Firewall-Configuration on windows

## Objective
The objective of this task is to configure and test basic firewall rules on a Windows system to understand how firewalls control and filter network traffic.

## Tool Used
- Windows Defender Firewall with Advanced Security

## Steps Performed

### 1. Listing Existing Firewall Rules
- Opened Windows Defender Firewall with Advanced Security.
- Viewed existing inbound firewall rules to understand current configurations.

### 2. Blocking Inbound Traffic on Port 23 (Telnet)
- Created a new inbound firewall rule.
- Selected TCP protocol and specified port 23.
- Configured the rule to block inbound connections on all network profiles.
- Named the rule "Block Telnet Port 23".

### 3. Testing the Firewall Rule
- Verified that inbound traffic on port 23 is blocked.
- Used command prompt to check port status.
- Confirmed that the firewall prevents connections to this insecure port.

### 4. Removing the Test Rule
- Deleted the temporary firewall rule to restore the system to its original state.

## Observations
- Firewalls control network traffic using predefined rules.
- Blocking unused or insecure ports reduces attack surface.
- Telnet (port 23) is insecure because it transmits data in plaintext.
- Firewall rules can be easily added, tested, and removed.

## Conclusion
This task helped in understanding basic firewall operations such as listing rules, blocking specific ports, testing firewall behavior, and restoring system configurations. Firewalls play a critical role in improving system and network security.
The firewall rule was tested using the netstat command. No active connections or listening services were found on port 23, confirming that inbound traffic to this port is blocked.
