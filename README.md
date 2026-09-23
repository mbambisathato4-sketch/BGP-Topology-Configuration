# BGP-Topology-Configuration
Configuring BGP across 4 autonomous systems

A simple illustration of how BGP is configure and routes are distributed between iBGP and BGP

## Network Topology

<img width="1280" height="587" alt="image" src="https://github.com/user-attachments/assets/ec1c806c-4b45-4880-8f93-72a3f43c2078" />

## Steps
- Assigned IP addresses to all interfaces
- Configured router IDs for each router.
- Set up 4 Autonomous Systems, one of which uses iBGP
- BGP is up and running on all routers across the topology

- ## Key configurations:

- Applied the Next-hop-self command on R2 for R1 to ensure proper routing.
- Implemented the route-reflector-client command on R2 to reflect routes within the AS.
With these configurations in place, R1 successfully learned all routes from BGP and was able to ping R5 without any issues

## Configuration Screenshots

R1

<img width="765" height="543" alt="image" src="https://github.com/user-attachments/assets/ce90fab7-a027-42db-93b8-821213b0e092" />
<img width="800" height="731" alt="image" src="https://github.com/user-attachments/assets/f275476e-5917-46ca-a991-4e384ad48cf2" />

R2

<img width="800" height="630" alt="image" src="https://github.com/user-attachments/assets/e22bd605-f43d-4ae7-adf3-ed34c01d6732" />
<img width="800" height="743" alt="image" src="https://github.com/user-attachments/assets/3e326517-276a-4d61-9e66-db0ea194e821" />

R3

<img width="800" height="770" alt="image" src="https://github.com/user-attachments/assets/0c4cdb9a-5fbf-493e-afc2-c590fb10e7d9" />

R4

<img width="800" height="827" alt="image" src="https://github.com/user-attachments/assets/dc8be96b-0087-4841-95ea-49534e10ed92" />

R5

<img width="800" height="661" alt="image" src="https://github.com/user-attachments/assets/30ff881b-3bb8-429f-8d37-bb473f2064ac" />

R6

<img width="800" height="619" alt="image" src="https://github.com/user-attachments/assets/1197fc43-9a62-4400-bdd9-226b4ae644af" />
