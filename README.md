# 💳 FacePay – Face Recognition Payment System (Final Year Project)

**FacePay** is an innovative payment system that uses **facial recognition technology** to authenticate users and process transactions securely without the need for physical cards or manual inputs. This system combines a **web application**, a **mobile app**, and a **desktop face scanner** to create a seamless and secure payment ecosystem.

---

## 🧠 Project Overview

The FacePay system is designed with the following core components:

1. **User Registration (Web)**  
   Users register by submitting personal details and facial data. Each user starts with 100 wallet points.

2. **Face Scanner (Desktop App)**  
   A separate face authentication application using **Haar Cascade** and **LBPH** algorithms. On successful scan, wallet points are deducted and transaction is recorded.

3. **Shopkeeper Dashboard (Web)**  
   View incoming transactions, customer details, and payment history in real time.

---

## 🏗️ Project Structure
Final_Year_Project_FacePay/
│
├── face_pay_web/ # Flask-based web app for registration & login
├── face_pay_scanner/ # Desktop face recognition scanner app
├── shop_website/ # Shopkeeper dashboard interface
└── database/ # SQLite databases (main and shop)


---

## ⚙️ Tech Stack

- **Frontend:** HTML, CSS, Bootstrap (web).
- **Backend:** Flask (Python), SQLite
- **Face Recognition:** OpenCV (Haar Cascade + LBPH)
- **Database:** SQLite3 (local), Firebase (optional)

---

## 🔐 Features

- 👤 Facial recognition-based user authentication
- 💼 Wallet with point system (100 points on sign-up)
- 🧾 Transaction history logging
- 🛒 Shopkeeper view for monitoring payments
- 🖥️ Desktop face scanner for real-time verification
- 📱 Android app for mobile registration and account management

---

## 🚀 How to Run

### 💻 Web App (Flask)

bash
<pre>
cd face_pay_web
pip install -r requirements.txt
python app.py
</pre>

### 🖥️ Face Scanner App
  
bash
<pre>
cd face_pay_scanner
python face_scanner.py
</pre>

---
  
### 🌐 Shopkeeper Dashboard

bash
<pre>
cd shop_website
python app.py
</pre>

## ⚠️ Ensure the shop.db and main user database are in the correct paths.

---
---
  
  
### 🧪 Facial Recognition Details
  - Detection: Haar Cascade Classifier
  - Recognition: Local Binary Pattern Histogram (LBPH)
  - Training: Model trained on registered facial data stored in trainer.yml

---
  
### 💡 Future Enhancements
  - 🔐 Integrate OTP/email verification during registration
  - 💳 Link to real banking APIs instead of wallet points
  - ☁️ Deploy the entire system on cloud (Firebase, Heroku, or AWS)
  - 📊 Add analytics dashboard for shopkeepers

