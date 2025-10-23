---
title: Email Hashing and Anonymous Participation Codes
layout: default
---

# 🔐 How We Protect Your Email

When you choose to enter your email address at the end of a planeasy-webgis questionnaire, it is used **only to generate an anonymous participation code**.  
This code allows us to recognize repeated participation across different surveys without ever storing or seeing your real email.

---

## 🧭 Why we ask for an email

- To **link responses** across multiple questionnaires (e.g., Profile + Safety + Trip Diaries) and understand how perceptions evolve over time.  
- To enable **longitudinal research** on mobility habits and safety behaviour.  
- To ensure the data remain usable for research without exposing any personal identity.

Providing an email is **completely optional**.  
If you skip this step, your responses remain fully anonymous and cannot be linked to future surveys.

---

## 🧮 How we protect and anonymize it

We apply a one-way cryptographic hash using the **SHA-256** algorithm combined with a secret salt.

### Example process

1. You enter your email (e.g. `alex@example.com`).
2. The app immediately computes: hash = SHA256(SALT + email.toLowerCase().trim())
3. Only the resulting code (e.g. `7d4a8e3f1b2c...`) is stored with your answers.  
4. The plain email is **never saved**, **never transmitted**, and **never shared**.

The **salt** is a secret key stored only in the application environment (not in the database).  
It ensures that even if two participants use the same email, their hash values differ between research instances.

---

## 🔒 Data protection principles

- **Pseudonymization**: The hash is a random-looking code that cannot be reversed to the original address.  
- **Data minimization**: Only the hash is stored; no identifiable fields remain.  
- **Purpose limitation**: The code is used exclusively for research data linkage within theBIKEnet and related scientific studies.  
- **Security**: All transmission and storage are encrypted (HTTPS / Firestore encryption at rest).

---

## 🧾 Compliance and transparency

This process follows the principles of:
- [GDPR, Article 89 – Processing for scientific research purposes](https://gdpr.eu/article-89-processing-for-scientific-research-purposes/)
- [FAIR data standards](https://www.go-fair.org/fair-principles/)

It ensures that participation in theBIKEnet and planeasy-webgis surveys is **ethical, secure, and scientifically valid**.

---

📎 *For more information about what we collect and why, see the [Data Collection Overview](data-collection.md).*  
📎 *For a plain-language summary of your privacy rights, see [Privacy Easy](privacy-easy.md).*

