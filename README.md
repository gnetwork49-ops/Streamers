# Streamers🎥
this is the platform where the voice of the people is hear in the world

A prototype social media platform for sharing posts, comments, and streams.

## 🚀 Getting Started

### Prerequisites
Make sure you have these installed on Ubuntu:
```bash
sudo apt update && sudo apt install git python3-pip nodejs npm postgresql
git clone https://github.com/gnetwork49-ops/Streamers.git
cd Streamers
cd backend
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
cd frontend
npm install
npm start
CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    username VARCHAR(50) UNIQUE NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    password_hash TEXT NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE posts (
    id SERIAL PRIMARY KEY,
    user_id INT REFERENCES users(id),
    content TEXT NOT NULL,
    media_url TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
---

👉 This gives you a **ready-to-paste README.md** with installation steps, backend/frontend setup, and a starter database # Sign up a new user
curl -X POST http://localhost:8000/signup \
  -H "Content-Type: application/json" \
  -d '{"username":"israel","email":"israel@example.com","password":"securepass"}'

# Create a new post
curl -X POST http://localhost:8000/posts \
  -H "Authorization: Bearer <token>" \
  -d '{"content":"Hello Streamers!"}'backend/   # Django API
frontend/  # React UI
docs/      # Documentation
git add README.md
git commit -m "Add setup instructions and schema to README"
git push origin main
## 🔧 Usage Examples

Once the backend is running on `http://localhost:8000`, you can test the API with `curl`:

### 1. Sign Up a New User
```bash
curl -X POST http://localhost:8000/signup \
  -H "Content-Type: application/json" \
  -d '{"username":"israel","email":"israel@example.com","password":"securepass"}'
curl -X POST http://localhost:8000/login \
  -H "Content-Type: application/json" \
  -d '{"username":"israel","password":"securepass"}'
curl -X POST http://localhost:8000/posts \
  -H "Authorization: Bearer <token>" \
  -H "Content-Type: application/json" \
  -d '{"content":"Hello Streamers!"}'
curl -X GET http://localhost:8000/posts \
  -H "Authorization: Bearer <token>"

## 📂 Project Structure

---

## 🚀 Why This Matters
- Makes your repo approachable for new developers.  
- Shows where backend vs frontend code lives.  
- Sets the stage for adding more modules (messaging, notifications, etc.).  
.
git add README.md
git commit -m "Add project structure section to README"
git push origin main
Enumerating objects: ...
Counting objects: ...
Compressing objects: ...
Writing objects: ...
To github.com:gnetwork49-ops/Streamers.git
   abc123..def456  main -> main

);

