This **README.md** is designed to provide a high-authority, "Wikipedia-level" overview of your project, incorporating the specific technical requirements for both the **FastAPI** backend and **Next.js** frontend.

---

# 🏢 Campus Resource Optimizer
### *Smart Utilization of Shared Campus Infrastructure*

The **Campus Resource Optimizer** is a centralized platform designed to track, predict, and optimize the usage of university resources. [cite_start]By addressing both spatial (labs, study rooms) and critical consumable (LPG, water) resources, the system ensures efficient campus operations and transparency for students and management alike[cite: 10, 79].

---

## 🚀 Key Features

* [cite_start]**Unified Resource Dashboard:** A single-pane view of all available labs, study spaces, and utility levels[cite: 33, 53].
* **Predictive Busyness Engine:** A "Smart" analytics endpoint that predicts resource congestion based on historical data and academic schedules.
* **Critical Consumable Tracking:** Real-time monitoring of vital infrastructure, including LPG cylinder counts and water tank levels.
* **Role-Based Access Control:** Distinct user experiences for **Students** (booking-focused) and **Management** (infrastructure-focused).
* **Responsive Dark Mode UI:** A premium, high-contrast interface designed to work seamlessly from mobile devices to large monitors.

---

## 🛠 Tech Stack

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Frontend** | **Next.js (App Router)** | High-performance, SEO-friendly React framework. |
| **Styling** | **Tailwind CSS & shadcn/ui** | Utility-first CSS and modern UI components. |
| **State Management** | **Zustand** | Lightweight, scalable state handling for role-switching and booking. |
| **Backend** | **Python (FastAPI)** | High-concurrency API with auto-generated Swagger documentation. |
| **Database** | **SQLite (SQLAlchemy)** | Reliable, lightweight relational database for quick deployment. |
| **Icons** | **Lucide React** | Clean, consistent iconography for a minimalist aesthetic. |

---

## ⚠️ Problem Statement

[cite_start]Modern university campuses often face challenges with **fragmented knowledge** and **disconnected resources**[cite: 10, 12, 19]:
1.  **Critical Shortages:** Extreme weather and global supply chain issues have caused unpredictable shortages in water and LPG cylinders.
2.  **Spatial Inefficiency:** Libraries and labs are often found full during exam cycles, while remaining underutilized at other times.
3.  [cite_start]**Manual Mismanagement:** New students often struggle with financial management and navigating complex booking schedules across disconnected tools[cite: 10, 22].

---

## 🏗 System Architecture

[cite_start]The platform follows a **modular and scalable architecture**[cite: 74, 80]:
* [cite_start]**Backend Hub:** Powered by FastAPI, acting as the central communication point for resource data and predictive services[cite: 74].
* **Service Layer:** Dedicated modules for resource listing, availability tracking, and "Smart" busyness prediction.
* [cite_start]**Frontend UI:** Built with Next.js to provide an interactive, responsive experience for all user roles[cite: 76].

---

## 📡 API Reference

| Endpoint | Method | Description |
| :--- | :--- | :--- |
| `/resources` | `GET` | Returns a list of all campus resources and current availability status. |
| `/book` | `POST` | Processes room bookings and prevents scheduling conflicts. |
| `/predict/{id}` | `GET` | **"Wow" Factor:** Returns a predicted busyness score (0-100%) for a resource. |
| `/admin/dashboard` | `GET` | Provides basic statistics (e.g., total bookings, popular resources). |

---

## 📥 Installation

```bash
# 1. Clone the repository
git clone https://github.com/tarun-sengar/campus-resource-optimizer.git

# 2. Setup Backend (Python 3.10+)
cd backend
pip install fastapi uvicorn sqlalchemy
python main.py  # This will auto-populate the database with 5 dummy resources

# 3. Setup Frontend
cd ../frontend
npm install
npm run dev
```

---

## 🗺 Future Roadmap

* **📡 IoT Integration:** Connecting ultrasonic sensors to automate water and LPG level updates.
* [cite_start]**🤖 AI Summarization:** Using LLMs to provide students with personalized "Best Time to Study" insights[cite: 83].
* [cite_start]**📊 Analytics Dashboard:** Providing management with long-term data on resource ROI and waste reduction[cite: 86].

---

## 👥 The Team: Vibe Coderz

* [cite_start]**Nilay Gurdasani [25BAI10563]**: Backend Developer [cite: 5, 91]
* **Keshav Maheshwari [25BAI11223]**: Frontend Developer
* [cite_start]**Tarun Sengar [25BAI11119]**: Documentation & QA [cite: 1, 87]

---
*Developed for the 2026 Hackathon Season.*