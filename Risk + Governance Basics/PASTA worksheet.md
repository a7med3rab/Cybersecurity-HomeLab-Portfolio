## PASTA worksheet

---

| Stages | Sneaker company |
| :---- | :---- |
| **I. Define business and security objectives** | Make **2-3 notes** of specific business requirements that will be analyzed. *Seamless buyer–seller marketplace with secure sign-up, login, and account management Strong data privacy and trust to protect user information and brand reputation Fast, reliable sales and payments with multiple options while meeting legal/regulatory requirements* |
| **II. Define the technical scope** | List of technologies used by the application: *Application programming interface (API) Public key infrastructure (PKI) SHA-256 SQL* The API is the highest priority because it directly handles user authentication, messaging, transactions, and data exchange with third-party services. APIs are frequent attack targets and expose large attack surfaces; weaknesses can lead to data breaches, unauthorized access, or payment fraud at scale. |
| **III. Decompose application** | [Sample data flow diagram](https://docs.google.com/presentation/d/1ol7y79popTFfNHM-90ES-H-i1Lpd0YNvPShxBlXozjg/template/preview?resourcekey=0-DZAkf7Vzh2PXsP-j3oXV-g) User searches sneakers → request sent via API API queries SQL database → retrieves listings Data returned to app → displayed to user Encryption (PKI, SHA-256) protects data in transit and at rest |
| **IV. Threat analysis** | List **2 types of threats** in the PASTA worksheet that are risks to the information being handled by the application. *External threat: API attacks (e.g., credential stuffing, injection, abuse of endpoints) Internal threat: Employee misuse or social engineering leading to unauthorized access*  |
| **V. Vulnerability analysis** | List **2 vulnerabilities** in the PASTA worksheet that could be exploited. *SQL injection vulnerabilities due to improper input validation Weak encryption or improper key management exposing payment or credential data* |
| **VI. Attack modeling** | [Sample attack tree diagram](https://docs.google.com/presentation/d/1FmWLyHgmq9XQoVuMxOym2PHO8IuedCkan4moYnI-EJ0/template/preview?usp=sharing&resourcekey=0-zYPY7AhPJdcClXamlAfOag) Threat actor targets API endpoint → exploits input validation flaw → gains database access → extracts user and payment data |
| **VII. Risk analysis and impact** | List **4 security controls** that you’ve learned about that can reduce risk. Strong authentication and multi-factor authentication (MFA) Secure API controls (rate limiting, input validation, authentication tokens) Encryption for data in transit and at rest (PKI, AES) Continuous logging, monitoring, and intrusion detection |

---

