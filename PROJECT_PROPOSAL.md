# 🐾 Capstone 2 Project Proposal — Home Fur Good 2.0

## **Description**
**Home Fur Good 2.0** is a full-stack web application that connects adoptable dogs with potential adopters.  
Inspired by Petfinder, this version expands on my original Flask project by rebuilding it in **React and Node.js** with a modern, interactive user experience.

Users can browse and filter adoptable dogs, favorite the ones they love, and submit adoption applications.  
A standout feature — the **“Least Loved Spotlight”** — highlights dogs with the fewest total favorites across all users, helping overlooked pets gain visibility.  
Admins can manage spotlighted dogs, view engagement data, and maintain adoption resources.

---

## **Tech Stack**
- **Frontend:** React, React Router, Axios, Context API, Tailwind CSS or custom CSS  
- **Backend:** Node.js, Express, PostgreSQL, JWT authentication  
- **External API:** Petfinder API (real-time adoptable dog data)  
- **Testing:** Jest, Supertest, React Testing Library  
- **Deployment:** Render or Vercel (frontend), Render or Railway (backend)  

---

## **Focus**
This will be an **evenly focused full-stack project**.  
The frontend emphasizes smooth UX, interactivity, and responsiveness, while the backend handles authentication, data persistence, and the logic behind favorites, applications, and spotlight rankings.

---

## **Type**
A **responsive web application**, optimized for both desktop and mobile browsers.

---

## **Goal**
To create a compassionate and engaging adoption platform that increases visibility for dogs in need of homes.  
Home Fur Good 2.0 aims to make it easy for users to:
- Find adoptable dogs that match their preferences  
- Favorite dogs they love and see real-time like counts  
- Learn about adoption and submit applications online  
- Help lesser-seen dogs gain attention through the **“Least Loved Spotlight”**

---

## **Users**
**Primary Users**
- Individuals and families looking to adopt  
- Volunteers or advocates promoting shelter dogs  
- Admins and shelter partners managing data and spotlight content  

The demographic includes adult pet lovers who are tech-savvy, compassionate, and motivated to support animal rescue and adoption.

---

## **Data**
- **Petfinder API:** Real-time data for adoptable dogs (name, breed, age, size, photos, status).  
- **Local Database:** Stores user accounts, favorites, adoption applications, and cached dog data for performance and analytics.

**Example Schema**
| Table | Key Fields |
|--------|-------------|
| **users** | id, username, email, password, is_admin |
| **dogs** | pf_id, name, breed, age, size, photo_url, status |
| **favorites** | user_id, pf_id |
| **applications** | id, user_id, pf_id, status, form_data |
| **dog_metrics** | pf_id, favorites_count, views_count |

---

## **Challenges & Considerations**
- Handling Petfinder API rate limits and syncing data efficiently  
- Securing JWTs and user credentials  
- Maintaining accurate favorite and view counts across all users  
- Ensuring accessibility and responsive design on all devices  

---

## **Core Functionality**
- User signup/login with JWT authentication  
- Browse, search, and filter adoptable dogs  
- Favorite/unfavorite dogs with live heart counters  
- Display total likes on each dog card  
- “Least Loved Spotlight” highlighting under-favorited dogs  
- Adoption application form and user dashboard  
- Admin metrics and resource management  

---

## **Stretch Goals**
- Email newsletter signup for new arrivals or adoption updates  
- Admin analytics dashboard for engagement metrics  
- Resource center for adoption and training guides  
- Progressive Web App (PWA) capabilities for offline access  

---

## **Summary**
**Home Fur Good 2.0** combines my passion for animal rescue with full-stack engineering.  
It’s a meaningful, data-driven platform designed not only to showcase adoptable dogs but also to give those most in need a better chance at finding their forever homes. ❤️
