
---

# ✅ **FILE 2: ARCHITECTURE.md (Complete New File)**  
This file contains the deep technical details — what developers expect when evaluating the architecture.

---

```markdown
# 🏗️ **AI-Resilience-Orchestrator — System Architecture**

This document provides a deep technical explanation of the internal design and operational flow of the AI-Resilience-Orchestrator.  
It is intended for:

- Cloud & distributed systems engineers  
- DevOps practitioners  
- AI/ML researchers  
- Open-source contributors  

---

# 📡 1. Detection Agent (Monitoring Layer)

The Detection Agent is responsible for **real-time system awareness**.

### **Key Responsibilities**
- Heartbeat checks (container → agent → orchestrator)
- Log scraping + anomaly detection
- Checksum validation for data integrity
- Latency + throughput metrics
- Pod/container health scoring

### **Data Flow**
