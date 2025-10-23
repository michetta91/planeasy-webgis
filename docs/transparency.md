---
title: Transparency and Data Protection – PlanEasy Framework
layout: default
---

# 🌍 Transparency and Data Protection  
### How PlanEasy Collects, Uses, and Protects Your Data

**PlanEasy** is an open research framework developed by [WEMO Lab](https://wemolab.eu) to support scientific studies and participatory mapping projects such as *theBIKEnet*.  
This page brings together all essential information on **what data we collect**, **why we collect it**, and **how we protect your privacy**.

---

## 🧭 1. What Data We Collect

We only collect the information that is essential for research and system operation — never for commercial use.  
Participation is voluntary and anonymous.

### 📝 Questionnaire responses
We collect answers about:
- **Profile** (age group, gender, education, employment, household context)  
- **Mobility habits** (how often you walk, cycle, or use public transport)  
- **Perceptions and experiences** (safety, comfort, infrastructure quality, incidents)  

> None of these fields identify you personally. You can skip any question you prefer not to answer.

### 📍 Spatial and mobility data (if you use an app)
Participants who use a related mobile app (e.g., *theBIKEnet*) may share:
- **GPS traces of trips** (location, time, duration)  
- **Trip purpose** (e.g., commute, leisure)  
- **Environmental notes or reports** (e.g., hazards, unsafe crossings)

> GPS data are automatically filtered and anonymized to remove areas near home or work.

### ⚙️ Technical metadata
Limited technical data ensure the system runs smoothly:
- Device or browser type  
- Submission timestamps  
- Anonymous session identifiers

---

## 💡 2. Why We Collect Data

Because real-world evidence helps design **better, safer, and more sustainable urban environments**.  
The data collected through PlanEasy are used to connect **citizen experience with urban decision-making**.

Researchers, practitioners, and local decision-makers use these data to:
- study mobility patterns and perceptions of public space,  
- evaluate infrastructure, accessibility, and safety,  
- compute indicators (KPIs) for planning and policy,  
- support participatory design and community dialogue,  
- and share anonymized results for educational, civic, and scientific purposes.

> 🧭 In PlanEasy, citizens act as *the eyes of the city* — their observations help professionals and institutions understand what works and what needs to change.

No data are ever used for marketing, profiling, or commercial purposes.

---

## 🔐 3. How We Protect Your Data

| Principle | What it means |
|------------|---------------|
| **Pseudonymization** | Every participant is identified only by a random internal code (or a hashed email, if provided voluntarily). |
| **Data separation** | Personal contact data (if collected) are stored separately from survey and GPS data. |
| **Encryption** | All data transfers use HTTPS; databases are encrypted at rest. |
| **Access control** | Only authorized research staff can view pseudonymized datasets. |
| **Transparency** | All documentation is public through the [planeasy-webgis repository](https://github.com/michetta91/planeasy-webgis). |

---

## ✉️ 4. How Email Hashing Works

When you optionally provide your email address at the end of a questionnaire, it is used **only to generate an anonymous participation code**.

### Process:
1. You enter your email (e.g., `alex@example.com`).  
2. The app computes: hash = SHA256(SALT + email.toLowerCase().trim())
3. Only the resulting hash (e.g., `7d4a8e3f1b2c...`) is stored with your answers.  
4. The plain email is never saved, transmitted, or shared.

### Why:
- To link your answers across multiple questionnaires (e.g., profile + trip diary)  
- To enable longitudinal research on mobility habits  
- To ensure data continuity without revealing personal identity

> Providing your email is **completely optional**.  
> If you skip it, your responses remain fully anonymous.

---

## 🧾 5. Legal and Ethical Context

Data are collected under the **GDPR Article 89** framework for *scientific research purposes*.  
Each project has its own designated **data manager** responsible for compliance and ethical oversight.

Participation is voluntary, and you may request data deletion at any time by contacting the research team.

---

## 🌍 6. Learn More

- [WEMO Lab website](https://wemolab.eu)  
- [GitHub Documentation – planeasy-webgis](https://github.com/michetta91/planeasy-webgis)  
- [Official Privacy Policy (theBIKEnet)](https://thebikenet.eu/privacy)

✉️ **Contact for data protection inquiries:**  
**privacy@wemolab.eu**

