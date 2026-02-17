# Azure Security Foundations

Labs focused on Azure RBAC, Key Vault, private endpoints, and Defender configuration.

Risk Identified:
Granting Owner access allows privilege escalation and data destruction.

Business Impact:
- Data loss
- Regulatory violations
- Service outage

# Azure RBAC & Least Privilege Lab

## Objective
Demonstrate risks of over-permissioned Azure RBAC roles and implement least privilege corrections.

---

## Initial Misconfiguration
Role: Owner  
Assigned To: dev-user  
Scope: Storage Account  

### Risk
Owner role allowed:
- Resource deletion
- Permission modification
- Privilege escalation
- Data destruction

### Business Impact
- Potential regulatory violations
- Loss of sensitive data
- Service disruption

---

## Remediation
Removed Owner role.
Assigned Storage Blob Data Contributor instead.

Security-user assigned Reader role for monitoring visibility.

---

## Logging & Audit Controls
Enabled diagnostic logging to ensure activity traceability.

---

## Key Lesson
Over-permissioning is one of the most common cloud security risks.
Least privilege significantly reduces blast radius.
