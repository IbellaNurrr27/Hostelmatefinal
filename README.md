# 🏨 HostelMate | Full-Stack Management System

![Status](https://img.shields.io/badge/Status-Production--Ready-success?style=for-the-badge)
![Score](https://img.shields.io/badge/Viva--Score-25%2F25-gold?style=for-the-badge)
![Sprint](https://img.shields.io/badge/Dev--Time-48--Hour--Sprint-blueviolet?style=for-the-badge)

> **A sophisticated, dual-sided portal for UET Lahore students and administrators. Built from scratch to automate the chaos of hostel allotments with real-time synchronization.**

---

## ✨ The Experience
HostelMate isn't just a database; it's a high-fidelity UX experience. 
* 🌌 **Interactive UI:** Features a custom 2D grid background that responds to cursor movement.
* 🔦 **Glow Aesthetics:** Consistent glow-shadow and hover effects across the entire interface.
* 📸 **Authentic Visuals:** All hostel imagery is hand-captured to ensure institutional trust.
* 👤 **Dynamic Personalization:** Real-time data fetching displays Student/Admin names, departments, and roommates immediately upon login.

---

## 🛠️ Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" />
  <img src="https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase" />
  <img src="https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/netlify-%23000000.svg?style=for-the-badge&logo=netlify&logoColor=#00C7B7" />
</p>

* **Frontend:** Vanilla JS (ES6+), Custom CSS3 animations, and Responsive Design.
* **Backend:** Firebase Firestore (NoSQL), Firebase Auth, and Firebase Storage.
* **Deployment:** Netlify (CI/CD).

---

## 🚀 Key Features

### 👨‍🎓 Student Side
* **Smart Registration:** Gender-specific filtering ensures students only see eligible hostels.
* **Auto-Allotment Engine:** Intelligent algorithm that fills halls sequentially to optimize utility.
* **Live Dashboard:** View roommate details, hall assignments, and roll numbers instantly.
* **Announcement Sync:** Real-time "Notice Board" updates pushed directly by Admins.

### 👩‍💼 Admin Side
* **Manual Override:** Full control to manually allot students to specific rooms regardless of auto-logic.
* **Mess Management:** Post daily mess schedules that instantly sync to relevant hostel dashboards.
* **Student Oversight:** Comprehensive view of all registered students, departments, and occupancy status.
* **Hall Control:** Automatic disabling of "Full" halls in the registration forms to prevent over-booking.

---

## 🏗️ Architecture & Logic
The project utilizes a **Relational NoSQL structure**. Even with high-concurrency requests, the system prevents double-booking through conditional Firestore queries:

1.  **Validation Layer:** Checks `current_occupancy` vs `max_capacity`.
2.  **State Management:** Disables selection UI if capacity is reached.
3.  **Role-Based Access:** Segregated data paths for `Admins/` and `Students/` collections.

---

## ⚡ The "3-Day Sprint" Story
This project was designed, developed, and deployed in **48 hours of pure focus**. 
* **The Pivot:** Midway through development, I migrated the entire architecture from a legacy PHP backend to **Firebase** to ensure real-time capabilities and better data integrity.
* **Solo Carry:** Handled the Full-Stack development, UI/UX design, Database Schema, and Documentation independently.

---

## 🔗 Live Demo
Check out the live project here: [HostelMate Official](https://hostelmateofficial.netlify.app/)

---

### 👨‍💻 Developed By
**Noor_ul_ain** *Passionate Full-Stack Developer | Problem Solver*

> "The difference between a grade and a career is the attention to detail."
