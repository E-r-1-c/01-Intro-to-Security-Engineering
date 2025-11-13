# Security Principles

## CIA Triad
The core principles of security every system should uphold:

- **Confidentiality**: Only authorized users can access information.
- **Integrity**: Data must remain accurate and unaltered.
- **Availability**: Information and systems must be accessible when needed.

## DAD (Opposite of CIA)
Represents what happens if security fails:

- **Disclosure**: Unauthorized access to information.
- **Alteration**: Unauthorized modification of data.
- **Destruction/Denial**: Data or services become unavailable.

## Fundamental Concepts of Security Models
Different frameworks enforce security in structured ways:

- **Bell-LaPadula Model**: Protects confidentiality  
  - "No Read Up, No Write Down"  
  - Prevents lower-level users from reading higher-level data and stops leaks downward.  

- **Biba Model**: Protects integrity  
  - "No Read Down, No Write Up"  
  - Stops lower-level data from contaminating higher-level data.  

- **Clark-Wilson Model**: Protects integrity via controlled operations  
  - Only authorized procedures can modify sensitive data.  
  - Uses **Constrained Data Items (CDIs)**, **Unconstrained Data Items (UDIs)**, **Transformation Procedures (TPs)**, and **Integrity Verification Procedures (IVPs)**.

- **Other Models**:  
  - Brewer and Nash, Goguen-Meseguer, Sutherland, Graham-Denning, Harrison-Ruzzo-Ullman (advanced or specialized applications).

## Defense-in-Depth
- Layer multiple security mechanisms to protect systems.  
- No single control is enough; overlapping protections reduce overall risk.

## ISO/IEC 19249 Principles
**Architectural Principles**: How to structure systems securely  
- **Domain Separation**: Isolate components to contain breaches.  
- **Layering**: Protect lower layers with multiple security checkpoints.  
- **Encapsulation**: Hide internal workings, expose only safe interfaces.  
- **Redundancy**: Backups to ensure availability and integrity.  
- **Virtualization**: Run isolated virtual environments to contain risk.  

**Design Principles**: How to configure and manage systems  
- **Least Privilege**: Grant only necessary access.  
- **Attack Surface Minimization**: Reduce entry points for attackers.  
- **Centralized Parameter Validation**: Validate all inputs from a single point.  
- **Centralized Security Services**: Keep critical functions manageable and secure.  
- **Error & Exception Handling**: Ensure failures don’t expose sensitive info.

## Zero Trust vs. Trust but Verify
- **Zero Trust**: Treat every user/device as untrusted until verified continuously.  
- **Trust but Verify**: Assume baseline trust but continuously monitor. Automated tools like IDS/IPS help enforce this.

## Threat vs. Risk
- **Vulnerability**: Weakness in a system.  
- **Threat**: Potential attacker or event that could exploit a vulnerability.  
- **Risk**: Likelihood and impact of a threat exploiting a vulnerability.  

**Mental Model:**  
Weak spot → Someone who could exploit it → Likelihood and impact
