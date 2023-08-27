# PowerShell

The RDP tool is still under development. 

The tool is designed to take network traffic which is downloaded into 
a .csv and use PowerShell to assist an an analyst in identifying potentially 
anomalous network traffic. The goal is to create a vector into investigating 
IP addresses of potential interest for exhibiting lateral movement of an
adversary. The script analyzes traffic from source IP to destination IP
and prints out the IPs with multiple hops within a network. Essentially,
if an IP which goes from point A to B, and that same IP goes from point B
to point C, that IP will be identified and can be investigated for further
analysis. 

This tool was created because of limited access for a certain network, in 
which only PowerShell was allowed. In its use case, it was to target 
traffic being potentially used by malicious RDP activity.

Note: This does not identify malicious activity. It only serves as a tool
to assist an analyst in identifying IP addresses which may or may not 
be worth investigating further. 
