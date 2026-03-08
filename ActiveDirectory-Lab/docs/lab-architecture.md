## Architecture Overview

```
Windows 11 Host
      │
VMware Workstation
      │
┌───────────────┐
│ DC01          │
│ Windows Server│
│ Active Dir +  │
│ DNS           │
└───────┬───────┘
        │
┌───────────────┐
│ Windows 10    │
│ Client VM     │
│ Domain Joined │
└───────────────┘
```
