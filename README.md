# 🙋‍♂️ Flask Get Current User API
---

🚀 **Need a ready-to-deploy version?**

Includes Docker, setup guide, sample responses, and full API structure.

👉 [Buy it on Gumroad](https://talabov.gumroad.com/)

---

A secure and minimal Flask API for retrieving the currently logged-in user using a JWT token. Ideal for adding `/me` endpoints to any auth system.

---

## ✅ Key Features

- 🔐 Get current user by JWT
- 🔎 Returns `id` and `email` from SQLite
- 🚫 Handles missing/invalid/malformed tokens
- 🧱 Includes error handlers and modular blueprint
- 🐳 Docker support

---

## 🚀 Endpoint

### Get Current User

**GET** `/me`

**Headers:**
```
Authorization: Bearer <your.jwt.token>
```

**Response:**
```json
{
  "id": 1,
  "email": "user@example.com"
}
```

---

## ⛔ Error Responses

```json
{ "error": "Authorization token missing or invalid" }

{ "error": "Unprocessable token or malformed request" }

{ "error": "User not found" }
```

---

## ⚙️ Requirements

```bash
pip install -r requirements.txt
```

- Flask  
- Flask-JWT-Extended  
- Flask-SQLAlchemy

---

## 🖥 How to Run

```bash
python app.py
```

Or using Docker:
```bash
docker build -t get-current-user-api .
docker run -p 5000:5000 get-current-user-api
```

---

## 🧪 Example Screenshots

- ✅ Valid JWT returns user info
- ⚠️ Invalid/missing token returns error
- 🧱 Token expiration respected

> See `/screens/` for Postman tests.

---

## 💼 Ready-to-Use Version

Includes JWT support, SQLAlchemy user model, and Docker integration:

👉 [Buy it on Gumroad](https://talabov.gumroad.com/)

---

## 📬 Contacts

- Email: talabov.ali72@gmail.com  
- Telegram: [@talabovali](https://t.me/talabovali)

---

**Need this in another language/stack (Node.js, Go, etc)?**  
Custom dev available — just reach out.
