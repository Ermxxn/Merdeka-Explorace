# 🇲🇾 Merdeka Explorace: Live Tracking & Checkpoint System

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white)

A real-time, mobile-responsive web application built to manage and track a campus-wide QR-code scavenger hunt. 
This project was developed and deployed to modernize campus events, eliminate paper trails, and create a highly engaging, competitive experience for participants.

## 🚀 How It Works
Instead of using passwords or staggered manual routing, the system uses a speed-run architecture:
1. **Scan & Snap:** Teams run to hidden physical locations and scan a unique QR code. 
2. **Verify:** The web portal opens, prompting the team to select their group name and upload an evidence photo directly from their mobile camera.
3. **Live Sync:** Upon submission, the time and image are securely logged to a PostgreSQL database.
4. **Rank:** A live leaderboard instantly updates via WebSocket, ranking teams based on completion speed and displaying their evidence photos in real-time.

## ✨ Key Features
* **Serverless Architecture:** 100% static frontend (HTML/CSS/JS) hosted easily on GitHub Pages or Netlify, connected directly to a BaaS (Backend-as-a-Service).
* **Live Real-Time Leaderboard:** Utilizes Supabase Realtime channels to automatically update rankings on the big screen without needing page refreshes.
* **Integrated Media Storage:** Captures environmental camera feeds on mobile devices and directly routes image buffers to secure cloud storage buckets.
* **Admin Command Center:** A dedicated control panel allowing event marshals to:
  * Wipe all progress logs to reset the game state.
  * Dynamically rename or scale the number of participating groups (up to 20).
  * Monitor and instantly delete spoofed/false check-in logs to maintain event integrity.
* **Immersive UI/UX:** Custom "Merdeka" theme utilizing glassmorphism, floating particle animations, and SweetAlert2 for tactile, high-energy user feedback.

## 🛠️ Tech Stack
* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **UI Framework:** Bootstrap 5
* **Backend / Database:** Supabase (PostgreSQL)
* **Storage:** Supabase Storage (Public Buckets for image handling)
* **Libraries:** SweetAlert2 (Popups), Canvas-Confetti (Micro-interactions)

## 📁 Repository Structure
* `checkpoint-[1-7].html` - The individual QR-scanned portals for each physical location.
* `leaderboard.html` - The live dashboard for Base Camp to track all teams.
* `admin.html` - The secure mission control center for JPP marshals.
* `LOGO JPP PMTG (1).jpg` - Asset file for the council branding.

## 👨‍💻 Developer
Developed by **Ermaan Singh**, Information Security student and member of the JPP PMTG board. 
