```markdown
# 🍔 Food Business Backend API

This is the standalone backend for a food ordering system built using Node.js and MongoDB, designed to support a small food business. Customers could browse food, create orders, add delivery addresses (Google Maps integration), and pay using PayPal. After successful orders, email confirmations are sent using Nodemailer.

---

## 📦 Project Overview

This backend powers:

- 🛒 Food ordering
- 📍 Google Maps-powered address handling
- 💳 PayPal payment integration
- 📧 Email notifications (Nodemailer)
- 🧾 Order management

This project was originally part of a full MERN stack application. The backend was developed separately.

---

## 🛠️ Tech Stack

| Tool         | Purpose                     |
|--------------|-----------------------------|
| Node.js      | Runtime                     |
| Express.js   | Web framework               |
| MongoDB      | Database                    |
| Mongoose     | ODM for MongoDB             |
| Nodemailer   | Email notifications         |
| PayPal REST API | Payments                |
| Google Maps API | Address geolocation     |
| Nodemon      | Dev environment live reload |

---

## 🚀 Setup & Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/food-api-backend.git
cd food-api-backend
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Create `.env` File

```env
PORT=5000
MONGO_URI=your_mongo_connection
PAYPAL_CLIENT_ID=your_paypal_id
PAYPAL_SECRET=your_paypal_secret
GOOGLE_MAPS_API_KEY=your_google_maps_key
EMAIL_USER=your_email@example.com
EMAIL_PASS=your_email_password
```

### 4. Run in Development Mode

```bash
npm run dev
```

---

## 📬 Core API Routes

| Route             | Method | Description                   |
| ----------------- | ------ | ----------------------------- |
| `/api/orders`     | POST   | Create a new order            |
| `/api/orders/:id` | GET    | Get order details             |
| `/api/address`    | POST   | Save user delivery address    |
| `/api/pay`        | POST   | Handle payment via PayPal     |
| `/api/send-email` | POST   | Send order confirmation email |

---

## 📧 Email Notifications

Nodemailer is used to send email confirmations once a client places an order. These include order summary, expected delivery time, and payment status.

---

## 📌 Notes

* Google Maps is used to convert user-entered addresses into valid delivery locations.
* PayPal sandbox credentials were used during development.
* Security and input validation were minimally handled for MVP purposes.

---

## 📜 License

MIT

---

## ✍️ Author

Developed by Thabani Ngwenya as part of a freelance/fullstack project.


