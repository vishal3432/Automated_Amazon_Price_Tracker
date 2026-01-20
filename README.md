# 🛒 Automated Amazon Price Tracker

A Python-based script that tracks an Amazon product’s price and sends an **email alert** when the price drops below a target value.
Built using **BeautifulSoup**, **Requests**, and **SMTP**, with credentials secured via **environment variables**.

---

## 🚀 Features

* Scrapes product **price & title** from Amazon
* Uses **custom headers** to avoid bot detection
* Converts price text into numeric format
* Sends **email notification** when price drops
* Secure credential handling using `.env`

---

## 🛠️ Tech Stack

* Python
* BeautifulSoup
* Requests
* smtplib
* python-dotenv

---

## 📂 Project Structure

```
amazon-price-tracker/
├── main.py
├── .env
└── README.md
```

---

## 🔐 Environment Variables

Create a `.env` file:

```env
SMTP_ADDRESS="smtp.gmail.com"
EMAIL_ADDRESS="your_email@gmail.com"
EMAIL_PASSWORD="your_app_password"
```

---

## ⚙️ How It Works

1. Sends request to Amazon with browser-like headers
2. Parses HTML using BeautifulSoup
3. Extracts product price and title
4. Compares price with target value
5. Sends email alert if price is lower

---

## ▶️ Run the Project

```bash
pip install requests beautifulsoup4 python-dotenv
python main.py
```

---

## ⚠️ Note

* Amazon pages change frequently
* Captcha may appear on live pages
---
