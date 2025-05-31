# 💼 Side Hustle & Money Quote API

This FastAPI project provides two simple but inspiring endpoints:

1. 🔁 `/side_hustles` — Returns a random idea for a side hustle.
2. 💬 `/money_quotes` — Returns a random motivational quote about money.

Both routes are protected using simple API keys.

---

## 🚀 How to Run

### 1. 📦 Install Dependencies

If you're using `uv`, run:

```bash
uv add fastapi[standard]
```

Otherwise with `pip`:

```bash
pip install fastapi "uvicorn[standard]"
```

### 2. 🏁 Start the Server

If you're using `fastapi-dev` or `fastapi dev`, run:

```bash
fastapi dev main.py
```

Or using Uvicorn:

```bash
uvicorn main:app --reload
```

📍 Server will be running at:
```
http://127.0.0.1:8000
```

---

## 🔐 API Endpoints

### ✅ `/side_hustles`

- **Method**: `GET`  
- **Description**: Get a random side hustle idea  
- **Query Parameter**:  
  - `apiKey` (required): `12345`

**Example**:
```
GET /side_hustles?apiKey=12345
```

---

### ✅ `/money_quotes`

- **Method**: `GET`  
- **Description**: Get a random motivational quote about money  
- **Query Parameter**:  
  - `apiKey` (required): `12345678911`

**Example**:
```
GET /money_quotes?apiKey=12345678911
```

---

## 📌 Notes

- ❗ Ensure you pass the correct `apiKey` in the query, or you'll get an "Invalid Key" response.
- 🛡️ This is a demo project for educational purposes. Avoid using hardcoded keys in production.

---

## ✨ Future Ideas

- [ ] Add `POST` endpoint for users to contribute new quotes/hustles
- [ ] Connect with a frontend using **Next.js** or **Streamlit**
- [ ] Store data in a database instead of static lists

---

## 🤝 Contribution

Pull requests and suggestions are welcome. Feel free to fork this repo and improve it.

---

## 📄 License

This project is open-source and available under the **MIT License**.