# 🚀 KoCourse — Realtime Certification Course Scrapper Portal (Django + Scraper)

KoCourse is a full-stack web application that automatically **scrapes certification courses** from multiple platforms and presents them in a **social media-style feed**. Users can explore, preview, and interact with courses through comments, likes, and bookmarks.

This version of the project is built using **Django + Python Scraper**, making it powerful for data extraction and backend processing.

---

## 📌 Features

* 🔍 **Automated Course Scraping**

  * Scrapes courses from platforms like Coursera, Udemy, edX
  * Extracts title, provider, duration, rating, and links
  * Runs periodically using background jobs

* 📰 **Social Media Feed UI**

  * Instagram/LinkedIn-style feed
  * Infinite scrolling
  * Clean card-based layout

* 💬 **Real-Time Comment System**

  * Add, reply, and like comments
  * Live updates using WebSockets (Django Channels)

* 👀 **Course Preview**

  * Detailed preview page with:

    * Description
    * Instructor info
    * Course content (if available)

* 🔐 **User Authentication**

  * Secure login/signup
  * Django authentication system
  * User profiles

* ⭐ **Like & Bookmark System**

  * Save favorite courses
  * Like courses
  * Track user activity

---

## 🛠️ Tech Stack

### **Backend**

* Django
* Django REST Framework
* Django Channels (WebSockets)

### **Frontend**

* React.js *(recommended)* OR Django Templates

### **Database**

* PostgreSQL *(recommended)*
* SQLite *(for development)*

### **Scraper**

* BeautifulSoup
* Scrapy *(optional for advanced scraping)*
* Selenium *(for dynamic websites)*

### **Task Queue (Optional but Recommended)**

* Celery
* Redis

---

## 🏗️ Project Structure

```id="r4mzcc"
KoCourse/
│
├── backend/                 # Django project
│   ├── kocourse/            # Main project settings
│   ├── courses/             # Course app
│   ├── users/               # User authentication
│   ├── comments/            # Comment system
│   └── api/                 # API layer (DRF)
│
├── frontend/                # React frontend (optional)
│
├── scraper/                 # Python scraping scripts
│
├── manage.py
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash id="m9q2js"
git clone https://github.com/your-username/KoCourse.git
cd KoCourse
```

---

### 2. Setup Backend (Django)

```bash id="s4g2vh"
cd backend
python -m venv venv
source venv/bin/activate   # (Windows: venv\Scripts\activate)
pip install -r requirements.txt
```

---

### 3. Configure Environment Variables

Create a `.env` file inside `backend/`:

```id="ykpl3h"
SECRET_KEY=your_secret_key
DEBUG=True
DB_NAME=kocourse
DB_USER=postgres
DB_PASSWORD=your_password
DB_HOST=localhost
DB_PORT=5432
```

---

### 4. Apply Migrations

```bash id="a8w7tc"
python manage.py makemigrations
python manage.py migrate
```

---

### 5. Run Development Server

```bash id="tn6r7c"
python manage.py runserver
```

---

### 6. Run Scraper

```bash id="y4k8zs"
cd scraper
python scraper.py
```

---

### 7. (Optional) Run Frontend

```bash id="yvl3h2"
cd frontend
npm install
npm start
```

---

## 🔄 Workflow

1. Scraper fetches course data periodically
2. Data is stored in PostgreSQL database
3. Django backend exposes REST APIs
4. Frontend displays courses in feed format
5. Users interact via comments, likes, bookmarks
6. Real-time updates handled using Django Channels

---

## 📊 Database Models (Overview)

* **User**

  * username, email, password

* **Course**

  * title, provider, duration, rating, link, description

* **Comment**

  * user, course, content, timestamp

---

## 🚧 Challenges

* Handling dynamic websites (requires Selenium)
* Avoiding duplicate course entries
* Managing real-time communication
* Scraping restrictions (CAPTCHA, rate limits)

---

## 🔮 Future Improvements

* 🤖 AI-based course recommendation
* 📱 Mobile application
* 🎓 Certificate verification system
* 📈 Analytics dashboard

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---



## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
