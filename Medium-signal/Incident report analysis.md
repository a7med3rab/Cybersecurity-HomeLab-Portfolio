**Incident report analysis**

| Summary | The organization experienced a Denial-of-Service (DoS) attack caused by a flood of ICMP packets entering through an unconfigured firewall, rendering internal network services unavailable for approximately two hours. The incident was mitigated by blocking ICMP traffic, offlining non-critical services, and restoring critical systems |  |  |
| :---- | :---- | ----- | ----- |
| Identify | An unconfigured firewall allowed unrestricted ICMP traffic Lack of rate limiting and spoofed IP detection No prior alerting on abnormal ICMP traffic volumes Network availability is identified as a critical asset  Primary risk: **network availability disruption via volumetric attack**  |  |  |
| Protect | Implement firewall rules to **rate-limit ICMP packets** Enable **source IP address verification** to block spoofed traffic Harden firewall baseline configurations Document firewall standards and review regularly Reduces exposure to traffic-based DoS attacks   |  |  |
| Detect | Deploy **network monitoring software** to identify traffic anomalies Implement **IDS/IPS** to flag and filter suspicious ICMP patterns Configure alerts for abnormal traffic spikes Faster detection and validation of DoS activity   |  |  |
| Respond | Block malicious ICMP traffic at the firewall Isolate affected network services Restore critical systems first Analyze logs to confirm the attack vector and source behavior Update incident response procedures Containment \+ learning loop enabled   |  |  |
| Recover | Restore normal network operations Bring non-critical services back online in phases Validate firewall and IDS/IPS effectiveness post-incident Communicate the resolution to internal stakeholders Ensures resilience and operational continuity   |  |  |

---

| Reflections/Notes: Unconfigured controls are exploitable controls DoS attacks target availability, not data Proactive rate limiting \+ monitoring drastically lowers risk NIST CSF provides a clear loop: learn → harden → monitor → recover  |
| :---- |

