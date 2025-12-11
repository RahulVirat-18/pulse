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
🔧 Installation & Setup
Prerequisites
Python 3.x

MySQL Server

Git

Step 1: Clone the Repository
Bash

git clone [https://github.com/your-username/Pulse-News-App.git](https://github.com/your-username/Pulse-News-App.git)
cd Pulse-News-App
Step 2: Set Up Virtual Environment
Bash

python -m venv venv
# Windows
.\venv\Scripts\activate
# Mac/Linux
source venv/bin/activate
Step 3: Install Dependencies
Bash

pip install -r requirements.txt
Step 4: Configure Environment Variables
Create a .env file in the root directory and add your keys:

Ini, TOML

DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=pulse_db

NEWS_API_KEY=your_newsapi_key
SIGHTENGINE_USER=your_sightengine_user
SIGHTENGINE_SECRET=your_sightengine_secret

MAIL_USERNAME=your_email@gmail.com
MAIL_PASSWORD=your_app_password
Step 5: Database Setup
Open MySQL Workbench.

Run the schema.sql script (included in the repo) to create tables.

Run seed_db.py to populate initial news content (optional).

Step 6: Run the App
Bash

python app.py
Visit http://127.0.0.1:5000 in your browser.
