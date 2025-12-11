# ⚡ Pulse - AI-Powered Social News Network

**Pulse** is a modern, secure, and intelligent social news aggregation platform designed to combat algorithmic bias and unsafe content. Built with **Flask**, **MySQL**, and **AI-powered moderation**, Pulse delivers a premium user experience with a "Cyber-Luxury" aesthetic.

 

---

## 🚀 Key Features

### 🛡️ **Security & Identity**
- **Two-Factor Authentication (2FA):** Optional security layer using Email OTP.
- **Email Verification:** Secure signup process with 6-digit verification codes via SMTP.
- **Privacy Controls:** Switch between **Public** and **Private** accounts. Private profiles require "Follow Requests."

### 🤖 **AI Content Moderation**
- **Real-Time Scanning:** All user uploads (Images/Videos) are scanned instantly using the **Sightengine API**.
- **Safety Gate:** Content flagged as Nudity, Violence, or Offensive is automatically blocked before posting.

### 🌐 **The Social Ecosystem**
- **Chronological Feed:** No algorithmic bias. See posts in real-time order.
- **Smart Interactions:** - **Like & Dislike:** Mutually exclusive reactions (toggling one removes the other).
  - **Reposts:** Share news to your profile with full attribution to the original author.
  - **Comments:** Engage in discussions on any news card.
- **WhatsApp Integration:** Direct deep-link sharing for viral reach.

### 🎨 **Premium UI/UX**
- **Cyber-Luxury Theme:** A sophisticated Deep Black, Lavender, and Silver aesthetic.
- **Glassmorphism:** Modern, translucent card designs.
- **Responsive:** Fully optimized for Desktop, Tablet, and Mobile.

---

## 🛠️ Technology Stack

| Component | Technology Used |
| :--- | :--- |
| **Backend** | Python, Flask (Micro-framework) |
| **Database** | MySQL (Relational DB) |
| **Frontend** | HTML5, CSS3 (Custom Design), JavaScript (Vanilla) |
| **AI Engine** | Sightengine API (Content Moderation) |
| **Data Source** | NewsAPI (Global Headlines) |
| **Email** | SMTP (Gmail) for OTPs |

---

## 🏗️ System Architecture

```text
[ User Client ] <---> [ Flask Server ] <---> [ MySQL Database ]
(HTML/JS UI)          (Python Logic)         (User/Post Data)
                            |
                            v
                     [ External APIs ]
             (NewsAPI, Sightengine, SMTP)
