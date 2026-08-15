# AuthChain UAV Protocol

## 📌 Overview
AuthChain UAV is a lightweight authentication protocol designed for secure communication between **User Device (UD)**, **Control Node (CN)**, and **Unmanned Aerial Vehicle (UAV)**.  
It leverages **hash functions, XOR operations, nonces, and timestamps** to ensure confidentiality, integrity, and mutual authentication in UAV networks.

---

## 🔐 Features
- **Nonce-based security** → prevents replay attacks.  
- **Timestamp validation** → ensures freshness of requests.  
- **Hash + XOR operations** → lightweight cryptographic primitives.  
- **Mutual authentication** → UD ↔ CN ↔ UAV all verify each other.  
- **Multi-factor ready** → supports constants like `Username`, `Password`, and `Biometric`.

---

## 📡 Protocol Flow
1. **UD → CN**: Sends authentication request with hashed/XORed values and timestamp.  
2. **CN → UAV**: Relays secure challenge using its own nonce and timestamp.  
3. **UAV → CN**: Responds with verification data tied to UD’s nonce.  
4. **CN → UD**: Confirms authentication back to UD.  
5. **CN → UAV**: Final secure acknowledgment to UAV.  

---

## ✅ Security Claims
- **Alive** → each role proves it is active.  
- **Nisynch** → prevents synchronization errors and replay.  
- **Niagree** → ensures agreement on exchanged values and session keys.  

---

## 🎯 Applications
- UAV communication in **IoT networks**  
- **Defense and surveillance systems**  
- **Smart city monitoring**  
- Lightweight security for **resource-constrained devices**

---

## ⚙️ Requirements
- Formal verification tools (e.g., AVISPA, ProVerif) for protocol analysis.  
- Basic knowledge of cryptographic primitives (hash, XOR, nonce).  
- UAV network simulation environment (optional for testing).  

---

## 🚀 Getting Started
1. Clone the repository:
   ```bash
   git clone https://github.com/Ajay9508/authchain-uav.git
   ```
   ## Tool
   - Scyther automation tool is used for formal verification of cryptographic protocols.
   -  The download link of the tool is:
     ```bash
     https://people.cispa.io/cas.cremers/scyther/
     ```
     ## Scyther-Manual
     - Scyther user manual link:
       ```bash
       https://ics.upjs.sk/~jirasek/krp/scyther-manual.pdf
       ```
       
