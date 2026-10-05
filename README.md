<div align="center">

# 🛠️ OPUS

### Service Management Platform for Cooperative Workers

*A web platform that connects customers with verified workers from cooperative societies, and manages the whole job: booking, assignment, OTP-verified start, proof of work, payment, ratings, complaints and worker welfare.*

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=white)

**[🌐 Live Demo](https://NAREIN29.github.io/OPUS/)**

</div>

---

## 🚩 The Problem

Hiring an electrician, plumber or AC technician still runs mostly on word of mouth.

- **Customers** can't easily verify who is coming to their home, or prove what work was done.
- **Workers** lack steady jobs, a formal identity, transparent earnings and welfare cover.
- **Cooperative societies** have no digital system to manage members, jobs and benefits.

## 💡 The Solution

OPUS puts cooperative societies at the centre. Every worker is approved by an admin, and every job follows a tracked lifecycle:

    Register → Admin approval → Booking → Worker assignment → OTP-verified start
       → Work completed with proof photo → Customer confirms → Payment → Rating

---

## ✨ Features

### 👤 Customer
- Register, log in and book a service with a **live price estimate**
- Share location so the nearest workers can be found (distance in km)
- **Recurring bookings** for regular services
- Track each request on a **status timeline**
- Give a **6-digit OTP** to the worker to start the job
- View the worker's **proof-of-work photo**, confirm completion and pay
- **Rate** the worker, **chat** with them, and raise **complaints**
- Download an **invoice** for each job

### 🧰 Worker
- Register with skills and location, and log in with a **Worker ID**
- Receive job assignments with in-app and **push notifications**
- Verify the customer's OTP to start a job, then upload a **proof photo** on completion
- See an **earnings breakdown** and view their **certificate**
- Enrol in **welfare and insurance** schemes

### 🏛️ Admin (Cooperative Society)
- **Approve or reject** worker registrations, with an approval stamp
- **Assign workers** to requests, ranked by skill and distance
- Worker directory, complaint resolution, and welfare records
- **Demand forecast**: requests by service type and day of the week
- Built-in **roadmap** showing what is implemented and what needs third-party integration

### 🌐 Across the app
- **English and Tamil** language support
- **Realtime** notification bell and chat
- Role-based access for customer, worker and admin

---

## 🏗️ Architecture

    Single-page web app (HTML + CSS + JavaScript)
    Customer view · Worker view · Admin view · English/Tamil
                         │
                         │ supabase-js
                         ▼
    Supabase: Auth · PostgreSQL · Realtime (chat, notifications)
              Storage (proof photos, documents) · RPC functions

### Database tables
`profiles` · `worker_profiles` · `cooperative_societies` · `service_requests` · `worker_assignments` · `service_pricing` · `recurring_bookings` · `payments` · `ratings` · `complaints` · `chat_messages` · `notifications` · `push_subscriptions`

---

## 🧰 Tech Stack

| Layer | Technologies |
|---|---|
| **Frontend** | HTML5, CSS3, Vanilla JavaScript (single-page app) |
| **Backend** | Supabase: PostgreSQL, Auth, Realtime, Storage, RPC |
| **Browser APIs** | Geolocation, Notifications, Service Worker (push) |
| **Hosting** | GitHub Pages |

---

## 🚀 Run Locally

    git clone https://github.com/NAREIN29/OPUS.git
    cd OPUS
    open index.html

The app connects to Supabase using the public **anon** key. Access to data is controlled with Supabase Row Level Security.

---

## 🗺️ Roadmap

- [x] Role-based auth and dashboards (customer, worker, admin)
- [x] Worker approval, Worker IDs and certificates
- [x] Booking, assignment, OTP start and proof-of-work photos
- [x] Chat, notifications, ratings, complaints and invoices
- [x] Recurring bookings and demand forecasting
- [x] Welfare and insurance enrolment
- [ ] Real payments through Razorpay (needs a server-side function for the secret key)
- [ ] Android app version
- [ ] More Indian languages

---

## 👤 Author

**Narein Muthukumaran**
B.E. Computer Science and Engineering, Saveetha School of Engineering · SIH 2025 Runner-Up

[LinkedIn](https://www.linkedin.com/in/narein-muthukumaran-s-524920402) · nareinsen29@gmail.com

---

<div align="center">

⭐ If you like this project, consider giving it a star!

</div>
