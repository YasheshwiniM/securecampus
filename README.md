# securecampus
A Passwordless Authentication for University Campus
# 🔐 SecureCampus —  MVP

Biometric Student Access Control System


## ✅ Run Instructions 

### Step 1 — Install Node.js 
Download from https://nodejs.org (LTS version)

### Step 2 — Enter project folder
```bash
cd securecampus
```

### Step 3 — Install dependencies
```bash
npm install
```

### Step 4 — Start the server
```bash
npm start
```

### Step 5 — Open in browser
Visit: http://localhost:3000



## 🗺️ User Flow

1. **Register** — Enter name, Student ID, and password → Create account
2. **Login** — Enter Student ID + password → Proceed
3. **Biometric** — Click "Scan Fingerprint" → Wait for "Biometric Verified ✓"
4. **Dashboard** — Click Lab / Library / LMS → Access granted with timestamp log
5. **Logout** — Return to login screen



## 🏗️ Tech Stack

| Layer    | Tech                  |
|----------|-----------------------|
| Frontend | HTML + CSS + JS       |
| Backend  | Node.js + Express     |
| Storage  | In-memory (Map)       |
| Auth     | Session via JS state  |
| Biometric| Simulated (1.8s delay)|



## 📁 Project Structure


securecampus/
├── server.js          ← Express API server
├── package.json       ← Dependencies
├── README.md          ← This file
└── public/
    └── index.html     ← Full frontend (HTML + CSS + JS)




## 🔌 API Endpoints

| Method | Route           | Description              |
|--------|-----------------|--------------------------|
| POST   | /api/register   | Register new student     |
| POST   | /api/login      | Login existing student   |
| POST   | /api/biometric  | Simulate biometric scan  |
| POST   | /api/access     | Log resource access      |



