# Missing Hardening

Hardening reduces a system's attack surface by removing unnecessary features, services, and access points. Without proper hardening, OT systems present a larger attack surface than required, increasing vulnerability to compromise.

## Description

System hardening is the process of securing infrastructure by minimizing attack vectors through:

- **Service reduction**: Removing unnecessary services, protocols, and interfaces
- **Access control**: Disabling default accounts and implementing proper authentication
- **Configuration management**: Applying secure defaults and security patches
- **Defense in depth**: Adding protective layers like firewalls and monitoring

OT environments face unique hardening challenges due to operational requirements for continuous availability and legacy system constraints that limit patching flexibility.

## Rationale

Hardening was included in the OWASP OT Top 10 based on empirical evidence showing:

- Missing hardening was a common factor in successful OT exploits
- Comprehensive hardening would have prevented many documented attacks
- The critical need for security layers in systems requiring continuous operation

While hardening doesn't eliminate specific vulnerabilities, it significantly increases exploitation difficulty and provides protective barriers during incident response.

## Known Attacks

**Stuxnet (2010)**: USB port hardening could have prevented initial compromise via infected removable media.

**NotPetya (2017)**: Proper endpoint hardening and disabling unnecessary services could have prevented lateral movement through compromised systems.

**Colonial Pipeline (2021)**: Hardened remote access systems and disabled default credentials could have prevented initial compromise.

## Mitigation Strategies

### For Developers/Suppliers/Integrators

**Design Phase:**
- Start with established hardening benchmarks (CIS, DISA STIGs)
- Implement secure-by-default configurations
- Disable unnecessary interfaces (USB, Telnet, debug ports, web services)
- Include application allowlisting capabilities

**Implementation:**
- Provide comprehensive hardening documentation
- Create deployment guides with security configurations
- Ensure hardening measures don't impact operational requirements

### For Operators

**Planning:**
- Consult industry best practices and adapt to your specific environment
- Create golden templates for standardized hardening configurations
- Develop environment-specific hardening procedures

**Deployment:**
- Implement hardening requirements in procurement specifications
- Verify hardening through penetration testing or cybersecurity acceptance testing
- Document all applied hardening measures

**Operations:**
- Reapply hardening after maintenance activities
- Implement automatic verification tools to ensure ongoing compliance
- Monitor for configuration drift using automated scanning
- Maintain hardening documentation and change control

## Implementation Steps

1. **Assessment**: Identify applicable hardening standards for your environment
2. **Planning**: Develop hardening implementation roadmap
3. **Implementation**: Apply hardening measures systematically
4. **Verification**: Test and validate hardening effectiveness
5. **Maintenance**: Establish ongoing hardening management processes

## Standards and References

### Compliance Frameworks
- **IEC 62443-2-1:2024** - Component hardening (COMP 1.1)
- **IEC 62443-2-4:2024** - Hardening guidelines (SP.02.03)
- **IEC 62443-4-1:2018** - Security hardening guidelines (12.4 SG-3)
- **NIST CSF 2.0** - Protect function (PR.PS)
- **EU NIS2 Directive** - Annexes 6.3, 6.9, 12.3

### MITRE ATT&CK Mitigations
M0806, M0818, M0921, M0924, M0927, M0928, M0934, M0936, M0938, M0942, M0944, M0949, M0950, M0951, M0954

### Hardening Resources

**Configuration Benchmarks:**
- **CIS Benchmarks**: Operating systems, network devices, applications
- **DISA STIGs**: DoD-standard security configurations
- **Microsoft Security Baselines**: Windows and Microsoft application settings

**Assessment Tools:**
- **Tenable Nessus**: Compliance scanning and vulnerability assessment
- **CIS-CAT Pro**: Automated benchmark assessment
- **Microsoft Security Compliance Toolkit**: Windows hardening verification

**OT-Specific Guides:**
- Vendor hardening documentation (e.g., Siemens SICAM/SIPROTEC hardening guides)
- Industry-specific hardening frameworks
- System integrator security implementation guides

### Additional Information
- [Computing Hardening Overview](https://en.wikipedia.org/wiki/Hardening_(computing))
- [Defense in Depth Strategies](https://en.wikipedia.org/wiki/Defense_in_depth_(computing))
