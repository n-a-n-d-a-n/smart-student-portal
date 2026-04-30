# Secure Whistleblower Platform Policy (Redline Draft — Illustrative)

> IMPORTANT: Illustrative only, not legal advice.

**Document ID:** SWP-POL-001  
**Version:** 0.9-Redline  
**Effective Date:** [DATE]  
**Owner:** [Security Office]  
**Legal Owner:** [General Counsel / Media Counsel]

## 1. Purpose
1.1 This policy governs the collection, handling, retention, access, and legal-process response for submissions to the whistleblower platform.  
1.2 The policy is designed to reduce source attribution risk while preserving lawful compliance obligations.  
**[COUNSEL NOTE: Confirm alignment with jurisdiction-specific press protections and organizational editorial charter.]**

## 2. Scope
2.1 Applies to all systems, personnel, and vendors processing platform data.  
2.2 Applies to production, staging, backups, logs, and audit systems where platform data may exist.  
**[COUNSEL NOTE: Decide whether to explicitly include affiliates, freelancers, and foreign bureaus.]**

## 3. Data Classification
3.1 **Class A (Highly Sensitive):** submission content (ciphertext and any plaintext during review).  
3.2 **Class B (Sensitive Operational):** workflow metadata, role actions, legal-hold metadata.  
3.3 **Class C (Operational):** aggregate non-identifying metrics.  
**[COUNSEL NOTE: Map classes to existing corporate data taxonomy if one exists.]**

## 4. Data Minimization and Prohibited Identifiers
4.1 The platform must collect only data necessary for service operation and editorial workflow.  
4.2 Prohibited-by-default fields include source IP, full user-agent, persistent device/browser fingerprints, and equivalent direct-attribution identifiers.  
4.3 Exceptions require written approval by Security + Legal + Editorial Standards, time-bounded, with purge plan.  
**[COUNSEL NOTE: Add jurisdiction-specific restrictions for “indirect identifiers” and metadata correlation.]**

## 5. Retention and Deletion
5.1 **Illustrative defaults:**  
- Submission ciphertext: 24 months  
- Workflow metadata: 24 months  
- Immutable audit events: 36 months  
- Security telemetry aggregates: 12 months  
5.2 Deletion must be automated where feasible and auditable.  
5.3 Legal hold may suspend deletion only for scoped records and must be reviewed every 90 days.  
**[COUNSEL NOTE: Validate durations against statutory limitation periods, litigation risk, and newsroom policy.]**  
**[COUNSEL NOTE: Confirm whether preservation duties may attach before formal service in any jurisdiction.]**

## 6. Access Control and Identity Assurance
6.1 Access is least-privilege, need-to-know, default-deny.  
6.2 Privileged access requires hardware-backed MFA/WebAuthn and managed-device posture checks.  
6.3 Sensitive actions (bulk export, out-of-scope decrypt, retention override) require dual authorization.  
6.4 Role recertification occurs quarterly; offboarding deprovision target is <4 hours.  
**[COUNSEL NOTE: Confirm employment-law implications for device posture requirements across regions.]**

## 7. Role Definitions (Illustrative)
7.1 **Platform Administrator:** infra operations; no default plaintext access.  
7.2 **Editorial Reviewer:** case review within assignment scope.  
7.3 **Key Custodian:** controlled key operations under dual control.  
7.4 **Legal Reviewer:** legal-demand intake, hold management, disclosure authorization.  
7.5 **Security Analyst:** security telemetry review without default content access.  
**[COUNSEL NOTE: Confirm segregation-of-duties sufficiency for regulator/court expectations.]**

## 8. Logging, Audit, and Monitoring
8.1 Logging must avoid prohibited identifiers by default.  
8.2 Privileged actions must generate immutable audit events.  
8.3 Audit tamper alerts trigger incident response immediately.  
**[COUNSEL NOTE: Verify admissibility and evidentiary standards for audit records in target jurisdictions.]**

## 9. Legal-Demand Handling (Subpoena/Order/Warrant)
9.1 All legal demands must be routed to Legal Intake; technical teams must not respond directly without counsel authorization.  
9.2 Counsel verifies authenticity, jurisdiction, enforceability, and scope before any preservation or production action.  
9.3 Any disclosure is limited to minimum legally compelled scope.  
9.4 Where lawful and appropriate, counsel will seek narrowing/challenge of overbroad requests.  
9.5 Chain-of-custody documentation is mandatory for preserved/produced records.  
**[COUNSEL NOTE: Add country/state-specific rules for notice obligations, gag orders, and contempt exposure.]**  
**[COUNSEL NOTE: Define external-counsel trigger thresholds (e.g., national security orders, extraterritorial requests).]**

## 10. Notification and Transparency
10.1 Notification to affected sources/users will be provided when legally permissible.  
10.2 If delayed by gag/seal restrictions, counsel will schedule periodic legality re-checks.  
10.3 Organization publishes aggregate legal-demand transparency reports [cadence: semiannual].  
**[COUNSEL NOTE: Confirm if transparency reporting creates additional legal/operational risk in your jurisdictions.]**

## 11. Incident Response and Breach Handling
11.1 Trigger events include unauthorized access, key compromise suspicion, prohibited-identifier persistence, and major availability incidents.  
11.2 Response includes triage, containment, preservation, remediation, and post-incident review.  
11.3 Legal and regulatory notifications follow applicable law and contractual obligations.  
**[COUNSEL NOTE: Add precise notice timelines by jurisdiction; include sector-specific breach rules if applicable.]**

## 12. Vendor and Third-Party Controls
12.1 Critical providers require security/privacy due diligence and contractual controls.  
12.2 Contracts must address breach notice timing, subprocessors, and data handling limits.  
12.3 Contingency and exit plans must exist for critical providers.  
**[COUNSEL NOTE: Confirm data-processing addenda and cross-border transfer mechanisms (if any).]**

## 13. Training and Awareness
13.1 Privileged users must complete annual training on source protection, legal-demand escalation, and secure handling.  
13.2 Completion and acknowledgment are mandatory and auditable.  
**[COUNSEL NOTE: Confirm mandatory training language with labor/union constraints where relevant.]**

## 14. Exceptions and Risk Acceptance
14.1 Exceptions require documented risk, compensating controls, and approval by CISO + General Counsel.  
14.2 Exceptions expire automatically unless renewed with explicit approval.  
**[COUNSEL NOTE: Add board/audit-committee notification threshold for high-impact exceptions.]**

## 15. Enforcement
15.1 Violations may result in access removal, disciplinary action, contract remedies, and/or legal action.  
**[COUNSEL NOTE: Align sanctions language with HR policy and collective bargaining obligations.]**

## 16. Governance and Review
16.1 Policy review cadence: semiannual or upon material legal/technical change.  
16.2 Material updates require Security + Legal joint approval.  
**[COUNSEL NOTE: Define “material change” with objective triggers.]**
