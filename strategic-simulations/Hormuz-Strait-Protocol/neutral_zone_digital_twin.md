# Neutral Zone Digital Twin (NZDT)
## Executive Summary
A sovereign-agnostic, high-fidelity simulation of the Hormuz Strait that forces all littoral and extra-regional powers to share real-time sensor data under cryptographic attestation. The twin continuously fuses sonar, radar, AIS, and SIGINT feeds into a single, tamper-evident operational picture that flags anomalous behavior 90 seconds before it can escalate to live fire. By making deception more expensive than transparency, the system converts the strait from a zero-sum chokepoint into a mutually-monitored commons.

---

## 1. Architectural Overview

### 1.1 Core Principle
**“Shared visibility precludes plausible deniability.”**  
Every submarine ping, helicopter radar sweep, or patrol-boat turn is time-stamped, cross-validated, and replicated across nine permissioned nodes before it can be weaponized as a surprise.

### 1.2 System Components
| Layer | Function | Latency Budget | Redundancy |
|-------|----------|----------------|------------|
| **Edge Mesh** | Sensor ingestion, local attestation | < 300 ms | 3× path |
| **Fusion Core** | Multi-sensor correlation, anomaly scoring | < 600 ms | 5× consensus |
| **Dissemination Bus** | Real-time broadcast to all stakeholders | < 200 ms | 9× nodes |
| **Digital Ledger** | Immutable audit trail, dispute evidence | < 2 s | 11× replicas |

---

## 2. Sensor Grid Topology

### 2.1 Mandatory Hardware Inventory
Each participating nation must deploy and maintain:

- **2× Passive Sonar Arrays** (seabed, 120° coverage)
- **1× OTH Radar** (3-30 MHz, 500 km range)
- **1× AESA Surface Radar** (X-band, 360°)
- **1× AIS Base Station** (VHF, 40 nm)
- **1× SIGINT Node** (HF/VHF/SHF intercept)

Failure to stream raw data at ≥ 1 Hz results in **cryptographic shaming**: the node’s public key is published on the ledger as “non-cooperative,” and its vessels lose NZDT-derived collision-avoidance guarantees.

---

## 3. Anomaly Detection Engine

### 3.1 Threat Vectors & Detection Logic
| Vector | Signature | Detection Window | Confidence |
|--------|-----------|------------------|------------|
| **Submarine Snorkel** | Periodic 3.5 kHz ping | 45 s | 94 % |
| **Fast Attack Craft** | >35 kn closing vector | 30 s | 97 % |
| **Mine Laying** | Speed drop + winch noise | 60 s | 91 % |
| **Drone Swarm** | 5+ radar tracks <50 m | 20 s | 99 % |
| **Radar Lock** | CW illumination >2 s | 15 s | 96 % |

### 3.2 Escalation Ladder
1. **Green**: Normal traffic variance (<2 σ)
2. **Amber**: Anomaly flagged, shared with all parties
3. **Red**: Predictive model triggers 90-second **“Pre-Emptive De-escalation”** broadcast
4. **Black**: Consensus threshold exceeded → automatic **“Safe Passage Corridor”** rerouting
