<div align="center">
  <h1>CAMPUS RESOURCE OPTIMIZER PROTOCOL [C.R.O.P]</h1>
  <h3><i>Smart Utilization of Shared Campus Infrastructure</i></h3>
</div>

<div align="center">
  <img src="https://via.placeholder.com/800x200?text=Campus+Resource+Optimizer+Banner" alt="Project Banner" width="800">
</div>

---

## 1. PROJECT OVERVIEW
The **Campus Resource Optimizer** is an integrated management system designed to address the critical challenges of resource allocation and infrastructure transparency within university environments[cite: 1]. [cite_start]The platform facilitates the real-time tracking, prediction, and optimization of both spatial assets (such as laboratories and study rooms) and essential consumable resources (such as LPG and water supplies)[cite: 1].

## 2. TEAM IDENTITY: VIBE CODERZ
<div align="center">

| Name | Role | Identification |
| :--- | :--- | :--- |
| **Nilay Gurdasani** | Backend Developer | 25BAI10563 |
| **Keshav Maheshwari** | Frontend Developer | 25BAI11223 |
| **Tarun Sengar** | Documentation & Quality Assurance | 25BAI11119 |

</div>

## 3. PROBLEM ANALYSIS
Contemporary campus management often suffers from fragmented data and lack of centralized visibility, leading to several operational inefficiencies:

* **Critical Infrastructure Scarcity**: Geopolitical factors and extreme weather conditions have resulted in unpredictable shortages of **LPG cylinders** and **water supplies**, necessitating real-time level tracking.
* **Spatial Underutilization**: Libraries and study rooms experience extreme "ghost booking" or overcrowding, particularly during disparate examination schedules across different academic years.
* **Management Complexity**: New students often face significant confusion regarding resource availability and financial management within the campus ecosystem.

## 4. PROPOSED SOLUTION
Our solution provides a unified digital library and resource manager where students and administrators can interact with campus infrastructure through a data-driven interface.

### Core Functionalities:
**Unified Resource Listing**: A comprehensive directory of all campus assets, categorized by type and capacity[cite: 1].
**Dynamic Availability Tracking**: Real-time status updates reflecting whether a resource is currently available, booked, or under maintenance[cite: 1].
**Intelligent Booking System**: A conflict-resolution engine that validates time-window requests to prevent overlapping reservations[cite: 1].
**Usage Insights Engine**: A predictive model that analyzes historical usage patterns to provide a **Busyness Score (0-100%)** for any given time-slot[cite: 1].

## 5. TECHNICAL ARCHITECTURE
The system utilizes a modular, scalable architecture to ensure high performance and low latency.

<div align="center">
  <img src="https://via.placeholder.com/600x300?text=System+Architecture+Diagram" alt="Architecture Diagram">
</div>

### Tech Stack Details:
| Layer | Technology | Rationale |
| :--- | :--- | :--- |
| **Frontend** | **Next.js (App Router)** | For responsive, server-side rendered user interfaces. |
| **Styling** | **Tailwind CSS** | Utilizing a high-contrast, premium dark-mode aesthetic. |
| **State Management** | **Zustand** | To handle role-switching and real-time UI state updates. |
| **Backend** | **Python (FastAPI)** | Chosen for high-speed performance and automated documentation. |
| **Database** | **SQLite (SQLAlchemy)** | For reliable relational data storage with minimal overhead. |

## 6. ROLE-BASED DIFFERENTIATION
The platform implements distinct visual and functional experiences based on the user's role:

* **Student View**: Optimized for individual productivity. Focuses on personal reservations, study room availability, and receiving high-level alerts regarding critical consumable shortages (e.g., Water/LPG alerts).
* **Management/Teacher View**: Optimized for administrative oversight. Provides granular data on resource levels (e.g., exact cylinder counts per hostel block), maintenance controls, and laboratory management.

## 7. API SPECIFICATIONS
The backend exposes several critical endpoints for frontend integration:

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/resources` | Retrieves all spatial assets and their current occupancy status. |
| `POST` | `/book` | Validates and creates a new resource reservation. |
| `GET` | `/predict/{id}` | Calculates the predicted congestion level for a specific resource. |
| `GET` | `/admin/dashboard` | Aggregates campus-wide metrics for administrative review. |

## 8. INSTALLATION AND SETUP
To deploy the project locally, follow these standardized steps:

### Backend Configuration:
```bash
pip install fastapi uvicorn sqlalchemy
python main.py