# Troubleshooting Notes

Common issues encountered during the lab:

DNS Misconfiguration
- Client machine could not locate the domain controller.
Solution:
- Set DNS server on the client to the IP address of the Domain Controller.

Group Policy Not Applying
- Policies were not immediately reflected.
Solution:
- Used gpupdate /force to refresh policies.

Network Connectivity Issues
- Verified network settings using:
  ipconfig
  ipconfig /all