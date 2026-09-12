# 🛡️ Azure Sentinel & KQL Threat Hunting Library

A curated repository of custom **Kusto Query Language (KQL)** queries designed for threat hunting, SOC detection engineering, and incident response across Microsoft Sentinel and Azure Active Directory (Microsoft Entra ID) environments[cite: 2].

---

## 🎯 MITRE ATT&CK® Mapping

| MITRE Technique | Tactics | Detection Query Link | Log Source |
| :--- | :--- | :--- | :--- |
| **T1110.001** | Initial Access / Brute Force | [Azure AD Password Spray](queries/initial-access/azure_ad_brute_force.kql) | `SigninLogs` |
| **T1098.003** | Privilege Escalation / RBAC | [High-Privilege Role Assignment](queries/privilege-escalation/azure_rbac_role_assignment.kql) | `AuditLogs` |
| **T1098.001** | Persistence / Cloud Credentials | [Service Principal Key Added](queries/persistence/service_principal_credentials.kql) | `AuditLogs` |

---

## 🛠️ How to Use These Queries

1. Open your **Microsoft Sentinel Workspace** or **Azure Log Analytics Workspace**.
2. Navigate to **Logs** or **Threat Hunting**.
3. Copy any `.kql` file from the `/queries` directory and adjust the timeframe (`ago(Xh)`) or detection thresholds as needed for your baseline.

---

## 👤 Author & Certifications

* **Author:** Chanbopich Tann[cite: 2]
* **Education:** M.S. in Cyber Security (UNCC) \| B.S. in Cyber Systems (USCGA)[cite: 2]
* **Certifications:** CompTIA Security+ (SY0-701), Microsoft SC-900, Microsoft AZ-900[cite: 2]
