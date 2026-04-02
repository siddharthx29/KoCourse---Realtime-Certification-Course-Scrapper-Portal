# KoCourse---Realtime-Certification-Course-Scrapper-Portal

# 🚀 KoCourse — Realtime Certification Course Scrapper Portal

KoCourse is a full-stack web application that automatically **scrapes certification courses** from multiple platforms and presents them in a **social media-style feed**. Users can explore, preview, and interact with courses through comments, likes, and bookmarks.

---

## 📌 Features

* 🔍 **Automated Course Scraping**

  * Fetches latest courses from platforms like Coursera, Udemy, and edX
  * Extracts title, provider, duration, rating, and course link

* 📰 **Social Media Feed UI**

  * Instagram/LinkedIn-style course feed
  * Infinite scrolling
  * Clean card-based layout

* 💬 **Real-Time Comment Section**

  * Add, reply, and like comments
  * Live updates using WebSockets

* 👀 **Course Preview**

  * Modal preview with:

    * Description
    * Instructor details
    * Syllabus (if available)
    * Embedded video (if available)

* 🔐 **User Authentication**

  * Secure login/signup system
  * JWT-based authentication
  * User profiles

* ⭐ **Like & Bookmark System**

  * Save favorite courses
  * Like courses
  * Track user activity

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Tailwind CSS
* Axios
* Socket.io-client

### Backend

* Node.js
* Express.js
* Socket.io

### Database

* MongoDB

### Scraper

* Python (BeautifulSoup / Scrapy) OR
* Node.js (Puppeteer)

---

## 🏗️ Project Structure

```
KoCourse/
│
├── client/             # React frontend
├── server/             # Node.js backend
├── scraper/            # Scraping scripts
├── models/             # Database schemas
├── routes/             # API routes
├── controllers/        # Business logic
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/KoCourse.git
cd KoCourse
```

### 2. Install dependencies

#### For backend:

```bash
cd server
npm install
```

#### For frontend:

```bash
cd client
npm install
```

---

### 3. Environment Variables

Create a `.env` file in the server folder:

```
PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
```

---

### 4. Run the application

#### Start backend:

```bash
cd server
npm run dev
```

#### Start frontend:

```bash
cd client
npm start
```

---

### 5. Run Scraper (optional)

```bash
cd scraper
python scraper.py
```

---

## 🔄 Workflow

1. Scraper collects course data periodically
2. Data is stored in MongoDB
3. Backend provides REST APIs
4. Frontend displays courses in feed format
5. Users interact via comments, likes, and bookmarks
6. Real-time updates handled using WebSockets

---

## 📷 Screenshots

> Add your UI screenshots here (Feed, Comment Section, Preview Modal)

---

## 🚧 Challenges

* Handling dynamic websites during scraping
* Avoiding CAPTCHAs and rate limits
* Maintaining real-time synchronization
* Ensuring scalable backend performance

---

## 🔮 Future Improvements

* 🤖 AI-based course recommendations
* 📱 Mobile application
* 🎓 Certificate verification system
* 📊 User analytics dashboard

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
