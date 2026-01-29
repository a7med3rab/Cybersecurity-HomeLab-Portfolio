# Security risk assessment report 

| Part 1: Select up to three hardening tools and methods to implement |  |
| :---- | ----- |
| **1\. Password Policies (NIST-aligned)** Enforce unique passwords per user Prohibit password sharing Require salting \+ hashing Eliminate default credentials, especially for admin/database accounts Network hardening tools \- Sheet1 **2\. Firewall Rules & Port Filtering** Define inbound/outbound rules based on business need Block unused ports Allow only required protocols and IP ranges Prevent unauthorized traffic flow Network hardening tools \- Sheet1 **3\. Multifactor Authentication (MFA)** Apply to employees, admins, and database access Use OTP, authenticator apps, or hardware tokens Protect against credential compromise Network hardening tools \- Sheet1 |  |
|  |  |

| Part 2: Explain your recommendations |
| :---- |
| **Password Policies** Directly fixes password sharing \+ default admin credentials Stops brute-force and credential-stuffing attacks Implementation: one-time rollout, quarterly audits, ongoing enforcement High impact, low cost **Firewall Rules & Port Filtering** Eliminates open attack paths Reduces attack surface immediately Blocks unauthorized ingress/egress traffic Implementation: initial configuration \+ continuous monitoring and updates Critical for perimeter defense **Multifactor Authentication (MFA)** Password alone becomes useless if stolen Proven reduction in account takeover risk Implementation: set once, maintain continuously Mandatory for admins and sensitive systems  |

