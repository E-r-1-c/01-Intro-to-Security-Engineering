# Identity & Access Management (IAM)

IAM is the framework and set of technologies used to manage digital identities, control access, and ensure accountability in an organization. It ensures the right people have the right access to the right resources at the right time.

---

## IAAA Model
The **four pillars of information security** that IAM addresses:

1. **Identification**  
   - How a user claims an identity (e.g., username, employee ID).  
   - Claiming an identity alone does not prove it is genuine.

2. **Authentication**  
   - Verifying that the claimed identity is valid.  
   - Methods:
     - **Something you know**: password, PIN, passphrase  
     - **Something you have**: security token, phone OTP, smart card  
     - **Something you are**: biometrics like fingerprint, retina, facial recognition  
     - **Multi-Factor Authentication (MFA)**: combines two or more factors for stronger security  
     - Lesser-used: **Somewhere you are** or **Something you do**

3. **Authorization**  
   - Determines what authenticated users are allowed to access and do.  
   - Enforced through **Access Control**.

4. **Accountability**  
   - Ensures users are responsible for actions they take.  
   - Achieved through **auditing and logging**.

---

## Access Control Models
1. **Discretionary Access Control (DAC)**  
   - Resource owners decide who gets access.  
   - Explicitly adds users; simple but less scalable for large organizations.

2. **Role-Based Access Control (RBAC)**  
   - Users are assigned roles; roles have permissions.  
   - Adding/removing users updates access automatically.  

3. **Mandatory Access Control (MAC)**  
   - Security-first model. Users cannot override permissions.  
   - Example: AppArmor on Linux.  

---

## Single Sign-On (SSO)
- Users log in once to access multiple systems.  
- Benefits:
  - One strong password and MFA.  
  - Fewer password resets.  
  - Improved efficiency and security.  

---

## Accountability & Logging
- Tracks user activities, system events, and errors.  
- Important for **compliance**, **incident response**, and **investigations**.  
- Logs should be **tamper-proof** and may be **forwarded** to central systems for monitoring.  
- **SIEM (Security Information and Event Management)**: Aggregates logs, detects anomalies, and flags potential threats.

---

## Identity Management (IdM)
- Manages digital identities for users and devices.  
- Covers identification, authentication, and authorization.  
- Ensures users have proper access while blocking unauthorized access.  

## IAM in Practice
- Centralized management of user identities, credentials, and access policies.  
- Enforces strong authentication, tracks activity, and ensures compliance with standards like **HIPAA, GDPR, PCI DSS**.  
- Protects sensitive resources while streamlining user experience.

