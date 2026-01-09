# 🍎 Calorie Tracker Pro

**Calorie Tracker Pro** is an AI-powered web application that analyzes food images to estimate **calories and macronutrients** (protein, carbs, fats). It combines a modern glassmorphic UI with computer vision and LLM-based reasoning to deliver an interactive, user-friendly nutrition tracking experience.

---

## 🚀 Project Overview

Tracking calories manually is time-consuming and error-prone. Calorie Tracker Pro simplifies this by allowing users to **upload or capture a food image**, automatically identify food items, and receive a **nutritional breakdown with visual insights**.

The app is fully frontend-based, lightweight, and deployable for free using static hosting platforms.

---

## ✨ Key Features

- 📸 **Image Upload & Camera Capture** (Web Camera API)
- 🤖 **AI-based Food Analysis** using Groq Vision (LLaMA models)
- 🔥 **Calorie & Macronutrient Estimation** per food item
- 📊 **Interactive Charts** (Pie / Doughnut / Bar) with Chart.js
- 🕘 **Analysis History Tracking** (LocalStorage)
- 📁 **CSV Export** for calorie history
- 🎨 **Dark / Light Theme Toggle**
- ⚙️ **Customizable Settings Panel**
- 🧊 **Glassmorphic UI** with Tailwind CSS

---

## 🧠 Tech Stack

### Frontend
- HTML5
- Tailwind CSS
- Vanilla JavaScript (ES Modules)

### AI & APIs
- **Groq API** (LLaMA Vision Models)
- **ImgBB API** (Temporary Image Hosting)

### Visualization
- Chart.js

### Analytics
- Firebase Analytics

### Storage
- Browser LocalStorage (History Persistence)

---

## 🏗️ System Architecture

### High-Level Architecture

```
User
  │
  ▼
Browser (UI)
  │
  ├─ Image Upload / Camera Capture
  │
  ▼
ImgBB Image Hosting
  │
  ▼
Groq Vision API (LLaMA)
  │
  ▼
JSON Nutrient Response
  │
  ▼
Charts + History + CSV Export
```

---

### Component Flow

```
UI Components
 ├── Image Input (Upload / Camera)
 ├── Preview Module
 ├── Analyze Button
 ├── Result Cards
 ├── Chart Modal
 ├── History Panel
 └── Settings Modal
```

---

## 🔄 Data Flow

1. User uploads or captures a food image
2. Image is uploaded to ImgBB
3. Image URL is sent to Groq Vision API
4. LLM returns structured nutrition JSON
5. App renders:
   - Food cards
   - Nutrient charts
   - History entries
6. Data is stored in LocalStorage
7. User can export data as CSV

---

## 📊 Visualization

- Pie / Doughnut / Bar charts
- Dynamic theme-aware rendering
- Interactive modal-based breakdown

---

## 🔐 Security Notes

⚠️ **Important:**
- API keys are exposed in the frontend (for demo purposes only)
- For production:
  - Use a backend proxy
  - Store keys securely in environment variables

---

## 🛠️ Installation & Usage

```bash
# Clone repository
git clone https://github.com/your-username/calorie-tracker-pro.git

# Open index.html directly in browser
```

No build tools or servers required.

---

## 📁 Project Structure

```
calorie-tracker-pro/
 ├── index.html
 └── README.md
```

---

## 🌱 Future Enhancements

- Backend proxy for secure API usage
- User authentication
- Daily calorie goals & progress tracking
- Food database integration
- Mobile PWA support
- Improved food recognition accuracy

---

## ⚖️ Disclaimer

This tool provides **approximate nutritional estimates** using AI models and should not replace professional dietary advice.

---

## ⭐ Support

If you find this project useful:
- ⭐ Star the repository
- 🍴 Fork it
- 🧠 Contribute improvements

---

## 👨‍💻 Author

**Ayan Chattopadhyay**

Built as a modern frontend + AI demo project showcasing computer vision, UI/UX, and API integration.
