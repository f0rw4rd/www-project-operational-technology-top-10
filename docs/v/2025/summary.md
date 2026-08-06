# Summary

OT runs the physical processes we all depend on: power plants, production lines, water treatment, medical devices. These systems are built for availability and safety, are operated for decades, and are now connected to office IT, their vendors, and often the internet.

When things go wrong in IT, the usual impact is data loss. When things go wrong in OT, production stops, equipment is damaged, and people can be hurt. The ten items below are the risks and missing practices our contributors keep running into, not individual vulnerabilities.

## The Top 10 at a Glance

1. **[Unknown Assets and Undocumented Services](the-top-10/unknown-assets-and-admin-access.md)**: If you cannot see it, you cannot patch, segment, or monitor it; undocumented services and forgotten remote access paths are how intruders reach the process.
2. **[(Accessible) Devices with Known Vulnerabilities/Issues](the-top-10/accessible-devices-with-known-vulnerabilities.md)**: Exposed devices with known vulnerabilities are easy, high-value OT targets. A single exploited PLC, HMI, or RTU can bypass upstream defenses and directly threaten the process.
3. **[Inadequate Supply Chain Management](the-top-10/inadequate_supply_chain_management.md)**: Vendors, integrators, and maintenance providers already have privileged access, so attackers use them to scale a single compromise across many operators.
4. **[Loss of Availability](the-top-10/loss-of-availability.md)**: Availability is the primary OT requirement. Outages can result from malware, unsafe changes, integrity failures, or faulty updates.
5. **[Insufficient Access Control](the-top-10/insufficient-access-control.md)**: Shared passwords, missing roles, and remote access without MFA let a single stolen credential become a path into the process.
6. **[Missing Incident Detection/Reaction Capabilities](the-top-10/missing-incident-detection-reaction-capabilities.md)**: Without logging, monitoring, and tested response, intrusions can persist unseen in OT environments for months and escalate from small incidents to major outages.
7. **[Broken Zones and Conduits Design](the-top-10/broken-zone-and-conduits-design.md)**: Flat networks allow one compromised host to reach many systems. The right zone design matches how the plant actually communicates and limits the blast radius.
8. **[Missing Awareness](the-top-10/missing-awareness.md)**: Controls must be understood and supported by operators. When staff do not know why a safeguard exists, it is bypassed or disabled to keep production running.
9. **[Components/Protocols with Insufficient Security Capabilities](the-top-10/components-with-insufficient-security-capabilities.md)**: OT systems last decades; selecting equipment or protocols without authentication, encryption, or update capability creates legacy risks that are difficult or impossible to remediate later.
10. **[Missing Hardening](the-top-10/missing-hardening.md)**: Hardening does not eliminate every vulnerability, but it increases the cost and difficulty of exploitation. In our experience, lack of hardening turned a vulnerability into a breach.

**Where to start.** The ranking is subjective. Get an inventory first, then address reachable and known-vulnerable systems, followed by segmentation and monitoring. [What’s next?](appendix/whats-next.md) has the concrete steps.
