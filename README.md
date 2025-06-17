# CHROME-EXTENSION-FOR-TIME-TRACKING-AND-PRODUCIVITY-ANALYTICS
TASK 4
Company Name : CODTECH IT SOLUTIONS

NAME : ADITYA PRATAP

INTERN ID : CT04DN802

DOMAIN : FULL STACK WEB DEVELOPMENT

DURATION 4 WEEKS

MENTOR : NEELA SANTOSH

# ⏱️ Productivity Tracker Chrome Extension

## Overview

**Productivity Tracker** is a real-time Chrome Extension built to help users monitor how they spend time across websites and improve productivity through data-driven insights. The tool tracks the time spent on each website, classifies them as productive or unproductive, and provides weekly analytics through an interactive dashboard. This project is built as part of the internship tasks at **CodTech**.

## 🔧 Key Features

- Tracks time spent on every visited domain in real-time.
- Differentiates between productive and unproductive websites.
- Stores user data securely using MongoDB.
- Backend developed using Node.js and Express.js.
- Interactive analytics dashboard built using React.js and Tailwind CSS.
- Weekly summary reports showing usage patterns.
- Extensible and lightweight Chrome Extension UI.

## 🛠️ Technologies Used

### Frontend:
- **React.js** for dashboard UI
- **Tailwind CSS** for styling
- **Chrome Extension API** (Manifest V3)

### Backend:
- **Node.js** with **Express.js** for RESTful API
- **MongoDB** for database
- **Mongoose** as MongoDB ODM

### Browser Extension:
- Manifest V3
- Background and Content scripts
- Fetch API to communicate with backend

## 🔗 Architecture

1. **Chrome Extension** tracks the active tab and records time spent.
2. When a tab changes, it sends the time data to the backend via a `POST /api/track` route.
3. All activity data is stored in MongoDB with timestamps.
4. The React dashboard fetches this data from `GET /api/analytics` and displays site-wise usage with productivity labels.
5. Reports are updated weekly, and the dashboard displays usage patterns visually.

## 📝 Productivity Classification

The extension classifies websites using a predefined list:

- **Productive**: Sites like `leetcode.com`, `stackoverflow.com`, `github.com`, etc.
- **Unproductive**: Sites like `youtube.com`, `instagram.com`, `facebook.com`, etc.

This logic can be easily modified or expanded inside the dashboard code.

## 🚀 Installation

### Chrome Extension:
1. Open `chrome://extensions` in your browser.
2. Enable “Developer mode”.
3. Click on “Load Unpacked” and select the `/extension` folder.

### Backend Server:
```bash
cd backend
npm install
node index.js
📩 Contact Email: singhaditya83475@gmail.com

LinkedIn: Aditya Pratap

GitHub: aditya-pratap01
