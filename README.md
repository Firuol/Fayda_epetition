# Fayda ePetition – National Platform to Raise and Track Citizen Petitions (with Blockchain Transparency)

## Contributors:
- Firaol Tesfaye
- Ermias Wakgari

---

## 🧩 Project Synopsis

### 🚨 Problem Statement
Ethiopia lacks a secure, centralized, and trustworthy platform for citizens to raise public or private petitions. Existing mechanisms are prone to fake entries, have no transparency, and do not allow petition tracking. Lack of a verified identity system has prevented meaningful civic engagement.

---

### 💡 Planned Solution
Build a **Flutter mobile app** that allows **Fayda-verified citizens** to:
- Raise petitions about public or private issues
- Sign petitions securely (one-person-one-signature)
- Track petition status and government responses
- Store a cryptographic hash of petitions, signatures, and responses on a blockchain ledger
- Enable transparent public participation without sacrificing identity privacy

---

## 🔐 Key Features

- ✅ Fayda ID & biometric authentication (VeriFayda OIDC)
- 🔏 Blockchain-based hash logging for tamper-proof history
- 📊 Trackable petition life cycle
- 👤 Public visibility (optional)
- 🧾 Comment and support other petitions
- 🛡️ Admin moderation and AI-powered flagging
- ⚖️ Government or company accountability portal

---

## 🔗 Blockchain Integration

| Component | Description |
|----------|-------------|
| **Platform** | Polygon (public) or Hyperledger Fabric (permissioned) |
| **Stored on Chain** | SHA-256 hash of petitions, signatures, and responses |
| **Verifiable** | Blockchain explorer to validate hashes of petitions |
| **Immutable Audit Trail** | No edits or deletions without trace |

### How it works:
- Petition content is hashed client-side → stored on-chain.
- Signatures hashed + timestamped → stored on-chain.
- Admin or authority response → hashed and logged.

---

## 👤 User Privacy

- Shows only **first name** + **last 4 digits** of Fayda ID
- Full identity and biometrics never exposed
- All blockchain hashes are anonymized (hash of content + user ID, not actual data)

---

## 🛠 Admin Role

- Approve/reject petitions
- Moderate flagged content
- Detect hate speech/misinformation via AI
- Ban accounts via Fayda ID (one-user-per-account)

---

## 🔐 Authentication & Identity

- Fayda-based registration via VeriFayda OIDC
- Biometric confirmation at first login
- One device/session per Fayda ID
- Signatures and petitions tied cryptographically to identity hash

---

## 🎯 Expected Impact

- Increased civic engagement
- Transparent public petitioning
- Trust between citizens and public offices
- Elimination of fake petitions or mass bot-signing
- Secure feedback loop from public to government

---

## 💼 Fayda’s Role

| Feature | Benefit |
|--------|---------|
| Identity Verification | Real users only, 100% trusted participation |
| Biometric Access | Prevents fraud or impersonation |
| One-person-one-account | Enforces fair civic participation |
| Masked Identity | Enables free speech with accountability |

---

## 💻 Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | Flutter |
| **Backend** | Node.js (Express) |
| **Authentication** | VeriFayda OIDC + Firebase Auth |
| **Database** | Firebase Firestore |
| **Blockchain** | Polygon or Hyperledger Fabric |
| **File Storage** | Firebase Storage / IPFS (optional future) |
| **Version Control** | GitHub |

---

