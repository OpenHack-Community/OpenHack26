# Project Name: Karwan

## Team Name

Triple Bytes

## Team Members

- Toufeeq Shaikh — [@toufeeqahmed916](https://github.com/toufeeqahmed916)
- Ayan Ali Shaikh — [@ayanalishaikh31-crypto](https://github.com/ayanalishaikh31-crypto)
- Ammar Talpur — [@ammartalpur](https://github.com/ammartalpur)

## Problem Statement

**CL-03 | Disaster Relief Resource Optimizer**

## Category

**Category 4: Climate & Disaster Resilience**

## Solution

Karwan is a disaster-relief coordination platform designed to help communities, coordinators, depot managers, and drivers work from one shared system during floods and other emergencies.

People can submit assistance requests by selecting their location, urgency, affected population, accessibility, and required supplies. Karwan gives each request a transparent priority score based on factors such as urgency, population, vulnerable groups, waiting time, and accessibility. Coordinators can then generate allocation recommendations based on available stock, demand, delivery capacity, truck availability, and distance.

Depot managers can maintain inventory for food, water, medicine, and shelter supplies, manage delivery vehicles, and review stock activity. Once an allocation is approved, it is assigned to a driver. The driver can start the trip and confirm delivery, while coordinators and requesters follow the same live progress on maps and dashboards.

Karwan also includes heatmaps, route visualization, low-stock warnings, delivery tracking, and a what-if simulator. The simulator lets coordinators test situations such as reduced stock, increased demand, capacity changes, and blocked roads before applying those changes.

The project uses simulated disaster data and focuses on making limited-resource decisions clear, explainable, and easy to demonstrate.

## Tech Stack

### Frontend

- React 18
- Vite
- React Router
- Tailwind CSS
- Leaflet and React Leaflet
- Leaflet Heat for heatmaps
- Supabase Realtime with polling fallback

### Backend

- Node.js 22
- Express.js 5
- REST APIs
- Vitest and Supertest for testing

### Database and Services

- Supabase PostgreSQL
- Supabase Realtime
- OSRM for road routes and distance estimates
- OpenStreetMap map data
- Vercel for frontend and backend deployment

## Challenges Faced

One of our main challenges was keeping the frontend and backend aligned while three team members worked on different features. We solved this by agreeing on API contracts first and developing the application phase by phase.

Resource allocation was another challenge because demand can be higher than available stock. We needed to consider urgency, affected population, distance, depot capacity, inventory, and truck availability while still giving coordinators a clear explanation for every recommendation.

Live delivery tracking also required extra work. Delivery progress had to remain synchronized across the driver page, coordinator dashboard, and requester tracker. Since the backend is deployed on a serverless platform, we changed the progress system to calculate movement from a saved trip start time instead of depending on a long-running server timer.

We also handled practical deployment issues such as CORS configuration, environment variables, database migrations, direct page refreshes with React Router, and keeping role-based sessions available after a refresh.

## Learnings

This project taught us that good coordination between team members is as important as writing code. Agreeing on the database structure and API contracts early allowed frontend and backend work to continue independently and reduced integration problems later.

We also learned how to turn a real-world problem into smaller development phases, build transparent scoring and allocation logic, manage shared application state, work with live database updates, test REST APIs, and deploy a full-stack application.

Most importantly, we learned that disaster-relief software should not only recommend an answer. It should also explain why that answer was recommended so that people can understand and trust the decision.

## AI / Open-Source Usage

### AI Tools

- OpenAI Codex was used as a development assistant for planning, debugging, code review, testing guidance, and documentation.

### Open-Source Tools and Resources

- React, Vite, React Router, and Tailwind CSS for the frontend
- Node.js and Express.js for the backend API
- Supabase JavaScript SDK for database and realtime communication
- PostgreSQL through Supabase for application data
- Leaflet, React Leaflet, and Leaflet Heat for maps and heatmaps
- OpenStreetMap for map tiles and geographic data
- OSRM for route calculation, distance, and estimated travel time
- Vitest and Supertest for backend testing

AI-assisted output was reviewed, tested, and integrated by the team. The project logic, feature decisions, database design, and final implementation remained under team control.

## Project Repository

[https://github.com/toufeeqahmed916/Karwan](https://github.com/toufeeqahmed916/Karwan)
