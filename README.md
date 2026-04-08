# 🌍 WanderWise: Personalized Travel Planner

**WanderWise** is a smart, sustainable, and social travel planning application designed to revolutionize how trips are organized. Developed as a DBMS Group Project at **IIITDM Jabalpur**, it moves beyond simple itinerary generation to offer eco-friendly options, group personalization, and smart context awareness.

---
## Contribution

This project was developed as part of a team of 6 members. I contributed by implementing the user module, including authentication, profile management, REST API development using Express, and MySQL-based storage for user preferences.

## 📖 Table of Contents
- [About the Project](#-about-the-project)
- [Core Features](#-core-features)
- [Project Modules](#-project-modules)
- [Tech Stack](#-tech-stack)
- [Database Schema](#-database-schema)
- [Contributors](#-contributors)

---

## 💡 About the Project

Travel planning is often fragmented across multiple apps for budgeting, routing, and reviews. WanderWise unifies these into a single platform. It uses data-driven insights to suggest itineraries based on budget, duration, and interests (nature, heritage, food, etc.).

What makes WanderWise unique is its focus on **sustainability** and **context awareness**. The system suggests itineraries based on the season/weather at the destination and calculates a "carbon footprint score" for each trip.

---

## 🚀 Core Features

### ✅ Smart Planning
* **Itinerary Generation:** Automates trip suggestions based on user constraints like budget and time.
* **Time Optimization:** Suggests the best routes and timings to maximize sightseeing.
* **Smart Context Awareness:** Avoids monsoon treks or suggests indoor activities based on weather data.

### 🌿 Sustainability & Social
* **Eco-Travel Mode:** Suggests sustainable travel options (public transport, eco-stays) and tracks carbon footprints.
* **Group Personalization:** Merges preferences from multiple users to create a balanced itinerary that satisfies both "foodies" and "trekkers".
* **Community Sharing:** Allows users to save, share, and rate itineraries (e.g., "Student Budget Goa Trip").

---

## 📦 Project Modules

The application is divided into 5 distinct modules to ensure modular development and clear separation of concerns:

1.  **User Module:** Handles authentication, user profiles, and preference settings.
2.  **Destination & Activity Module:** Manages the database of places, activities, associated costs, and seasonality data.
3.  **Itinerary Generator Module:** The core logic engine that processes Budget + Time + Preference to output a smart plan.
4.  **Community/Sharing Module:** Facilitates saving, sharing, and rating of itineraries among the user base.
5.  **Admin/Analytics Module:** A dashboard for monitoring user trends, popular destinations, and average budgets. Useful for tourism boards.

---

## 🛠 Tech Stack

* **Backend:** Express
* **Frontend:** React 
* **Database:** MySQL
* **External APIs:**
    * *OpenWeather API:* For weather-based context awareness.
   

---

## 🗄 Database Schema

The project utilizes a relational database designed to handle complex relationships between users, trips, and destinations.

**Key Entities:**
* **User:** Stores login credentials (`password_hash`), roles (User/Admin), and preferences.
* **Itinerary:** The central entity linking users to their planned trips, including attributes like `carbon_footprint_score` and `total_est_cost`.
* **ItineraryItem:** Represents specific activities within a trip with start/end times.
* **Destination & Activity:** Stores static data regarding locations, descriptions, and seasonality.
* **SharedItineraryReview:** Allows the community to rate and comment on public itineraries.

---

## 👥 Contributors

**Team Members (IIITDM Jabalpur)**

* **Pratik Prajapati**
* **Shraddha Singh**
* **Vinita Soni**
* **Priya Singh**

---

### 📝 License

This project was developed for academic purposes at IIITDMJ.
