# ⚡ Pulse - AI-Powered Social News Network

**Pulse** is a modern, secure, and intelligent social news aggregation platform designed to combat algorithmic bias and unsafe content. Built with **Flask**, **MySQL**, and **AI-powered moderation**, Pulse delivers a premium user experience with a "Cyber-Luxury" aesthetic.

---

## 🚀 Key Features

### 🛡️ Security & Identity
- **Two-Factor Authentication (2FA):** Email OTP security.
- **Email Verification:** 6-digit verification system using SMTP.
- **Privacy Controls:** Switch between **Public** and **Private** accounts with follow requests.

### 🤖 AI Content Moderation
- **Real-Time Content Scanning** using **Sightengine API**.
- Blocks **Nudity, Violence, Offensive Media** before posting.

### 🌐 The Social Ecosystem
- **Chronological Feed:** No algorithmic bias.
- **Smart Interactions:**
  - Like / Dislike (mutually exclusive)
  - Reposts with attribution
  - Comment system  
- **WhatsApp Deep-Link Sharing**

### 🎨 Premium UI/UX
- **Cyber-Luxury Theme:** Deep Black · Lavender · Silver  
- **Glassmorphism Cards**  
- **Fully Responsive**

---

## 🛠️ Technology Stack

| Component | Technology |
|----------|------------|
| Backend | Flask (Python) |
| Database | MySQL |
| Frontend | HTML, CSS, JavaScript |
| AI Engine | Sightengine API |
| News Source | NewsAPI |
| Email | Gmail SMTP |

---

## 🏗️ System Architecture

```text
[ Client ] <----> [ Flask Server ] <----> [ MySQL Database ]
                      |
                      v
              [ External APIs ]
      (NewsAPI, Sightengine, SMTP)
🔧 Installation & Setup
Below steps guide you through setting up Pulse on your system.

📥 1️⃣ Clone the Repository
 
Copy code
git clone https://github.com/your-username/Pulse-News-App.git
cd Pulse-News-App
🧱 2️⃣ Create & Activate Virtual Environment
bash
Copy code
python -m venv venv

# Windows
venv\Scripts\activate

# Mac/Linux
source venv/bin/activate
📦 3️⃣ Install Dependencies
bash
Copy code
pip install -r requirements.txt
🔐 4️⃣ Setup Environment Variables
Create a file named .env in the root project folder:

ini
Copy code
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=pulse_db

NEWS_API_KEY=your_newsapi_key
SIGHTENGINE_USER=your_sightengine_user
SIGHTENGINE_SECRET=your_sightengine_secret

MAIL_USERNAME=your_email@gmail.com
MAIL_PASSWORD=your_app_password

SECRET_KEY=your_flask_secret_key
🗄️ 5️⃣ Set Up the Database
Open MySQL Workbench

Run the following:

sql
Copy code
SOURCE database/schema.sql;
(Optional)

bash
Copy code
python database/seed_db.py
▶️ 6️⃣ Run the Application
bash
Copy code
python app.py
Now visit:

cpp
Copy code
http://127.0.0.1:5000
📂 Folder Structure
pgsql
Copy code
Pulse/
│
├── app.py
├── config.py
├── requirements.txt
├── .env
│
├── static/
│   ├── css/
│   ├── js/
│   └── uploads/
│
├── templates/
│   ├── login.html
│   ├── feed.html
│   └── profile.html
│
├── database/
│   ├── schema.sql
│   └── seed_db.py
│
└── utils/
    ├── sightengine.py
    ├── email_sender.py
    └── auth.py
