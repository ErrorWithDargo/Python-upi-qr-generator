# 🧾 Python UPI QR Code Generator

Generate UPI QR Codes using Python to accept payments from
PhonePe, Paytm, Google Pay and other UPI apps.

---

## 🚀 Features
- Generate UPI payment QR code
- Supports PhonePe, Paytm & GPay
- Beginner friendly Python project
- Clean & simple code
- Perfect for automation & freelancing

---

## 🛠 Requirements
- Python 3.7+
- qrcode library
- pillow library

Install dependencies:
```bash
pip install qrcode[pil]

## 🧑‍💻 Usage

import qrcode

upi_id = "yourupi@bank"
name = "Your Name"
amount = "100"

upi_link = f"upi://pay?pa={upi_id}&pn={name}&am={amount}&cu=INR"

qr = qrcode.make(upi_link)
qr.save("upi_qr.png")

print("UPI QR Code Generated Successfully")

