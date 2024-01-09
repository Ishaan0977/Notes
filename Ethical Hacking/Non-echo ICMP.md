- Instead of sending ICMP echo requests , the scanner sends out other types of ICMP messages
==Approach 1== : Send ICMP type 13 messages (Timestamp) by -PP option
- The scanner queires current time to the target
==Approach 2== : Send ICMP type 17 messages ( Address Mask Request) by -PM option
- The scanner queries subnet mask to the target
- This feature is sued by  diskless workstations during booting.