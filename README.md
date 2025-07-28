# Fayda ePetition – Verified National Petition Mobile Platform

## Contributors

- Firaol Tesfaye  
- Adding two more soon

---

## 📌 Project Synopsis

### Problem Statement  
Ethiopia currently lacks a **secure**, **transparent**, and **accountable** platform where citizens can raise and sign **petitions** targeting societal and governmental issues. Existing methods (social media, paper-based campaigns) are vulnerable to manipulation, fake accounts, and rarely lead to actionable results.

---

### Planned Solution  
Fayda ePetition is a **Flutter-based mobile application** integrated with **Fayda National ID** via **VeriFayda OIDC**, allowing:
- Citizens to **create**, **sign**, and **track petitions**
- Verified support (one person = one signature)
- Government agencies to **view and respond** to petitions
- End-to-end **transparency and accountability**

---

## 🔐 Fayda Integration

- **Authentication** is done via **VeriFayda OIDC**, ensuring:
  - One account per citizen
  - Biometric identity verification
  - No duplicate or fake users
- **Privacy Preserving:** Only the user’s **first name** and **region** are shown on petitions.

---

## 💡 Key Features

- ✅ Create and manage verified petitions
- ✅ Sign petitions using Fayda ID (only once per petition)
- ✅ Track petition status and progress
- ✅ Comment and support with regional identity
- ✅ Admin panel for moderation and validation
- ✅ Push notifications for petition updates

---

## 🧩 Expected Outcomes

- Foster **civic engagement** and a participatory democracy
- Eliminate **bot or spam-based petitioning**
- Provide **real-time, region-based** citizen feedback to authorities
- Amplify voices from **rural and underserved** areas
- Increase **trust and transparency** in public institutions

---

## 🛡️ User Privacy & Moderation

- **User Identity:** Only partial info (first name + region) is shown publicly
- **Moderation:** 
  - Admins can approve/reject petitions
  - Harmful or spammy petitions are flagged and removed
  - Repeat violators are permanently blocked using Fayda ID

---

## ⚙️ Tech Stack

### Mobile App (Frontend)
- **Flutter** (Dart)
- **Firebase Auth** (for session management)
- **Firebase Cloud Messaging** (notifications)
- **Firestore** (NoSQL real-time database)

### Backend (API)
- **Node.js** with **Express.js**
- REST APIs for:
  - Petition creation, update, deletion
  - Signature validation (linked to Fayda ID)
  - Admin moderation tools
  - Notifications and feedback
- **JWT Authentication**
- **VeriFayda OIDC** for national ID-based login

### Hosting
- Firebase Hosting (dashboard and docs)
- Railway/Render (Node.js API)
- Firebase Cloud Functions (optional)

### Version Control
- Git + GitHub

---

## 📁 Firestore Data Structure (Example)

