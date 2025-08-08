# Task 4: Setup and Use a Firewall on Windows

## Objective
Configure and test basic firewall rules to allow or block traffic.

## Tools Used
- **Windows Defender Firewall with Advanced Security**

## Steps Performed
1. Opened **Windows Defender Firewall with Advanced Security**.
2. Navigated to **Inbound Rules** → **New Rule**.
3. Selected **Custom Rule**, set **Protocol type** to `ICMPv4`.
4. Chose **Block the connection**.
5. Named the rule `Block_ICMP_Echo`.
6. Verified the rule appears in the Inbound Rules list.

## Testing Procedure
- **Before Blocking:** Ping from a friend's PC to my system was successful.
- **After Blocking:** Ping requests timed out, confirming ICMP was blocked.

## Screenshots
- `before-ping.png` – Before blocking ICMP (ping successful)
- `after-ping.png` – After blocking ICMP (ping failed)
- `firewall-rule-created.png` – Firewall rule configuration

## Conclusion
The firewall rule successfully blocked incoming ICMP Echo Requests, preventing other systems from pinging this PC.
