# 🌍 Nestrail

> **Stays along your journey**
> A full-stack travel accommodation platform built with Node.js, Express, MongoDB, and EJS — developed as part of my internship at **CodeAlpha**.

---

## 📸 Overview

**Nestrail** is an Airbnb-inspired travel accommodation platform where users can explore, create, edit, and review travel destinations across diverse categories such as Beach, Mountain, City, Castle, Camping, and more. Find comfortable places to stay at every stop of your journey.

---

## ✨ Features

- 🏠 **Full CRUD** – Create, Read, Update, and Delete travel listings
- ⭐ **Reviews & Ratings** – Add star ratings and feedback for any listing
- 🔍 **Search & Filter** – Search by destination title, city, or country
- 🏷️ **Category Filtering** – Filter by Beach, Mountain, City, Castle, Camping, Farm, Skiing, Arctic, Tropical, Desert
- 💰 **Price Sorting** – Sort listings by price (low to high / high to low) or newest
- 💾 **Wishlist** – Save favorite stays to localStorage
- 🚨 **Flash Messages** – Real-time toast notifications for actions and errors
- 📱 **Responsive Design** – Optimized for desktop, tablet, and mobile devices

---

## 🛠️ Tech Stack

| Layer       | Technology                        |
|-------------|-----------------------------------|
| Runtime     | Node.js                           |
| Framework   | Express.js                        |
| Database    | MongoDB + Mongoose                |
| Templating  | EJS (Embedded JavaScript)         |
| Styling     | CSS3                              |
| Sessions    | express-session + connect-flash   |
| Forms       | method-override (PUT/DELETE)      |
| Config      | dotenv                            |

---

## 📁 Project Structure

```
nestrail/
├── app.js              # Main application entry point
├── models/
│   ├── listing.js      # Listing Mongoose model
│   └── review.js       # Review Mongoose model
├── views/
│   ├── includes/       # Layout boilerplate, navbar, footer
│   └── listings/       # EJS templates (index, show, new, edit, wishlist)
├── public/             # Static assets (CSS, manifest.json)
├── init/               # Database seeding scripts & sample data
├── .env.example        # Environment variables template
└── package.json
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16+)
- [MongoDB](https://www.mongodb.com/) (running locally or MongoDB Atlas URI)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/soni015972/wanderlust.git

# 2. Navigate into the project
cd wanderlust

# 3. Install dependencies
npm install

# 4. Set up environment variables
cp .env.example .env
# Edit .env and configure your MONGO_URL and SESSION_SECRET

# 5. Seed the database (optional)
npm run seed

# 6. Start the development server
npm run dev
```

The app will run at **http://localhost:8080**

---

## 📝 API Routes

| Method | Route                             | Description             |
|--------|-----------------------------------|-------------------------|
| GET    | `/listings`                       | View all listings       |
| GET    | `/listings/new`                   | New listing form        |
| POST   | `/listings`                       | Create a listing        |
| GET    | `/listings/:id`                   | View listing details    |
| GET    | `/listings/:id/edit`              | Edit listing form       |
| PUT    | `/listings/:id`                   | Update a listing        |
| DELETE | `/listings/:id`                   | Delete a listing        |
| POST   | `/listings/:id/reviews`           | Add a review            |
| DELETE | `/listings/:id/reviews/:reviewId` | Delete a review         |

---

## 🎓 Internship

This project was built as part of my **Web Development Internship at CodeAlpha**.

---

## 📄 License

ISC © 2024 Nestrail