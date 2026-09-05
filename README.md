# 🛡️ Cyber Range Capstone — MySQL Honeypot & Threat Hunting Lab

> **An end-to-end cybersecurity lab focused on building, hardening, monitoring, detecting, hunting, investigating, and responding to real-world attacks against an internet-exposed MySQL server.**

---

## 🎯 Lab Overview

| Category                   | Environment                           |
| -------------------------- | ------------------------------------- |
| 🖥️ **Host**               | Windows Virtual Machine               |
| 🗄️ **Target Service**     | MySQL Server                          |
| 🛡️ **Endpoint Security**  | Microsoft Defender for Endpoint (MDE) |
| 📊 **SIEM**                | Microsoft Sentinel                    |
| 📜 **Telemetry**           | MDE Telemetry + MySQL Audit Logs      |
| 🔎 **Detection & Hunting** | KQL + Threat Hunting                  |
| 🌐 **Attack Surface**      | Controlled Internet Exposure          |

---

## 🔄 Defensive Lifecycle

```text
┌──────────────┐
│ 🛠️ BUILD    │
└──────┬───────┘
       ↓
┌──────────────┐
│ 🔒 HARDEN    │
└──────┬───────┘
       ↓
┌──────────────┐
│ 📡 INSTRUMENT│
└──────┬───────┘
       ↓
┌──────────────┐
│ 📊 BASELINE  │
└──────┬───────┘
       ↓
┌──────────────┐
│ 🔎 HUNT      │
│ & DETECT     │
└──────┬───────┘
       ↓
┌──────────────┐
│ 🔴 EXPOSE    │
└──────┬───────┘
       ↓
┌──────────────┐
│ 🚨 INVESTIGATE│
└──────┬───────┘
       ↓
┌──────────────┐
│ 🛡️ RESPOND   │
└──────────────┘
```

**Build → Harden → Instrument → Baseline → Hunt → Detect → Expose → Investigate → Respond**


🏗️🛡️ Honeypot Architecture & Security Design 

<img width="900" height="560" alt="sql" src="https://github.com/user-attachments/assets/0c2b9f93-b8af-41eb-ada1-60f52a1b65e3" />

---

# 🔎 Threat Hunting & Detection Overview

This Cyber Range Capstone simulates the complete defensive lifecycle of an internet-exposed asset from the perspective of a **Security Operations Center (SOC) Analyst, Threat Hunter, and Detection Engineer**.

The lab begins by securely configuring and hardening a Windows-based MySQL environment. Comprehensive telemetry is then enabled across the endpoint, database, and security monitoring layers to establish visibility before any malicious activity occurs.

A behavioral baseline is developed to understand normal system and database activity. Detection rules and proactive threat-hunting queries are created and validated **before the environment is exposed to the internet**.

Once monitoring and detections are operational, the environment is deliberately weakened and exposed in a controlled manner to generate realistic attacker activity.

The resulting telemetry is used to identify suspicious behavior, investigate attacker techniques, map activity to the **MITRE ATT&CK framework**, and document the incident lifecycle from initial access through response.

---

## 🎯 Defender Objectives

The primary objective of this lab is to ensure the defender has visibility **before, during, and after an attack**.

* 👁️ Establish comprehensive security visibility
* 📡 Collect and centralize endpoint and database telemetry
* 📊 Establish a baseline of normal behavior
* 🔎 Develop proactive threat-hunting hypotheses
* 🚨 Build and validate detection logic
* 🌐 Safely expose the environment to realistic attack traffic
* 🕵️ Investigate suspicious and malicious activity
* 🧩 Analyze attacker techniques and behavior
* 🎯 Map findings to the MITRE ATT&CK framework
* 📋 Document the complete investigation lifecycle
* 🛡️ Contain and respond to identified threats

---

## 🧠 Core Defensive Principle

> ### 🔴 **When the attack begins, the defender should already have visibility.**

This lab is not simply about deploying a honeypot.

It is designed to simulate a complete **SOC, Threat Hunting, and Detection Engineering workflow**, demonstrating how defenders prepare an environment, collect telemetry, establish baselines, detect anomalies, investigate attacker behavior, and respond to security incidents.

---

### 🛡️ Mission Statement

> **Build securely. Instrument completely. Understand normal behavior. Detect anomalies. Hunt proactively. Investigate thoroughly. Respond decisively.**
