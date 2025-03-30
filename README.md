# Web Application with Django & ReactJS

## 🛠 Tech Stack
- **Frontend:** React.js
- **Backend:** Django Rest Framework
- **Database:** PostgreSQL (or SQLite for local testing)

## 🚀 Features
- ✅ User Authentication (Email/Password Login)
- ✅ File Management (Upload, View, Download)
- ✅ Dashboard (File Analytics: Total Uploads, File Types Breakdown)
- ✅ User Profile (Edit Username, Manage Address & Phone)

---

## 📥 Installation & Setup

### Backend Setup (Django API)
```bash
# Clone the repository
git clone <repository_link>
cd backend

# Create a virtual environment and activate it
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt

# Set up the database
python manage.py migrate

# Create a superuser (optional for admin access)
python manage.py createsuperuser

# Start the Django server
python manage.py runserver
```

### Frontend Setup (React.js)
```bash
cd frontend

# Install dependencies
npm install

# Start the React development server
npm start
```

---

## 🔗 API Endpoints

### Authentication
```http
POST /api/auth/login/       # Login with email/password
POST /api/auth/register/    # Register a new user
```

### File Management
```http
GET  /api/files/              # List all uploaded files
POST /api/files/upload/       # Upload a new file
GET  /api/files/<id>/download/ # Download a file
```

### Dashboard
```http
GET /api/dashboard/summary/  # Fetch file upload statistics
```

---

## 🚀 Deployment (Optional)
```bash
# Build frontend
cd frontend
npm run build

# Use Docker for containerization
# Deploy with Heroku, AWS, or DigitalOcean
```

---

## 📂 Repository Link
[GitHub Repository](<insert_repo_link_here>)

---

## 📜 License
MIT License
