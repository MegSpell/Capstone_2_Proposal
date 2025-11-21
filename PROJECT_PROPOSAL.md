🐾 Home Fur Good 2.0
Capstone 2 Project Proposal
---------------

A modern adoptable-dog discovery platform built with React, Node, and the RescueGroups API.

---------------
📌 Project Description
---------------

Home Fur Good 2.0 is a full-stack web application that connects adoptable dogs with potential adopters. This version expands on my original Flask project by rebuilding it in React and Node.js for a cleaner, more interactive experience.

Users can browse and filter adoptable dogs, view detailed profiles, and favorite the ones they love.
A unique feature — the Least Loved Spotlight — highlights dogs with the fewest favorites across all users, giving overlooked pets a better chance at finding loving homes.

Admins can view engagement metrics, manage spotlighted dogs, and maintain rescue resources.
---------------
🛠️ Tech Stack
---------------
Frontend

React

React Router

Axios

Context API

Custom CSS

Backend

Node.js

Express

PostgreSQL

JWT authentication

External API

RescueGroups.org API (v5) for real-time adoptable dog data

Testing

Jest

Supertest

React Testing Library

Deployment

Frontend: Render

Backend: Render

---------------
🐶 Why the RescueGroups API?
---------------

The project initially explored Petfinder, however the Petfinder API is becing decomissioned and will no onger in use after December 2, 2025. RescueGroups offered more consistent data and broader rescue coverage just more difficulties matching request params so will be a learning curve but doable.

RescueGroups uses a strict JSON:API format, which introduced some challenges:

Requests must be sent as POST, even for searches

Headers must include:
Content-Type: application/vnd.api+json

Request body must be nested inside a data object

Filters require:

fieldName

operation

criteria

Location searches require a special filterRadius object

Once the structure was correct, the API became reliable and returned detailed dog listings perfect for this project.
---------------
🎯 Project Goals
---------------

Home Fur Good 2.0 aims to provide:

A modern, responsive platform for browsing adoptable dogs

A quick, friendly way to favorite dogs and see total like counts

A unique spotlight section for dogs receiving the least engagement

A seamless adoption-focused experience for both users and admins
---------------
👥 Target Users
---------------
Primary Users

Individuals or families looking to adopt

Dog lovers and rescue supporters

Admins and volunteers managing spotlight data

Users are typically adult pet lovers who value convenience, responsiveness, and clear design.
---------------
📊 Data Model
---------------
External (RescueGroups API)

Dog name, breed, age, size

Photo URLs

Rescue info

Location & distance

Status (Available/Pending)

Internal Database

Stores application-specific data such as:

Table	Key Fields
users	id, username, email, password, is_admin
favorites	user_id, dog_id
dogs	rg_id, name, breed, age, size, photo_url
dog_metrics	dog_id, favorites_count
⭐ Core Features

User signup/login (JWT authentication)

Browse adoptable dogs

Search & filter by breed, age, size, or location

Favorite/unfavorite dogs

Live favorite counters on each dog card

Least Loved Spotlight

Dog detail pages with rescue info and direct links

Admin dashboard with metrics and resource links

---------------
🚀 Stretch Features (Optional)
---------------

Email signup for new arrivals

Enhanced analytics for admins

Training & adoption resource center

Dog-of-the-Day feature

PWA capabilities
---------------
❤️ Summary
---------------

Home Fur Good 2.0 combines animal rescue advocacy with full-stack development.
The goal is to build a compassionate, user-focused platform that increases visibility for overlooked dogs and makes adoption simpler and more engaging.


















