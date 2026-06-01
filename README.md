# ShopNow — eCommerce App 🛒

<div align="center">

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-626CD9?style=for-the-badge&logo=stripe&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=for-the-badge&logo=redux&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

**Amazon-like full-stack eCommerce platform**

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| 🔐 **JWT Auth** | Register, login, protected routes |
| 🔍 **Product Search** | Search, category filter, price range, sort |
| 🖼️ **Image Gallery** | Product detail with multiple images |
| ⭐ **Reviews & Ratings** | Star ratings (1–5) by logged-in users |
| 🛒 **Shopping Cart** | localStorage persistence |
| 💳 **Stripe Checkout** | Secure payment processing |
| 📦 **Order Tracking** | Status steps (Pending → Shipped → Delivered) |
| 👤 **User Profile** | Shipping address management |
| ❤️ **Wishlist** | Toggle products to wishlist |
| 📊 **Admin Dashboard** | Sales analytics with charts |
| 🛠️ **Admin CRUD** | Manage products, orders, users |
| ☁️ **Cloudinary** | Image upload & storage |
| 📄 **Pagination** | Products and orders pagination |
| 🐳 **Docker** | Full-stack Docker Compose deployment |

---

## 🛠️ Tech Stack

### Frontend
- **Next.js 14** — React framework with App Router
- **Redux Toolkit** — State management
- **Tailwind CSS** — Styling
- **Stripe.js** — Payment UI

### Backend
- **Node.js** + **Express** — REST API
- **MongoDB** + **Mongoose** — Database
- **JWT** — Authentication
- **Cloudinary** — Image storage
- **Stripe** — Payment processing

---

## ⚡ Quick Start

### 1. Backend
```bash
cd backend
npm install
cp .env.example .env
# Fill in your .env values
npm run dev
```

### 2. Seed Database
```bash
npm run seed          # Import sample data
npm run seed -- -d    # Destroy all data
```

**Sample accounts:**
- Admin: `admin@example.com` / `admin123`
- User: `john@example.com` / `john123`

### 3. Frontend
```bash
cd frontend
npm install
cp .env.local.example .env.local
npm run dev
```

### 4. Docker (All-in-one)
```bash
cp backend/.env.example backend/.env
docker-compose up --build
```

---

## 🌐 URLs

| Service | URL |
|---|---|
| Frontend | http://localhost:3000 |
| Backend | http://localhost:5000 |
| API Health | http://localhost:5000/api/health |

---

## 💳 Stripe Test Cards

| Card | Scenario |
|---|---|
| `4242 4242 4242 4242` | ✅ Success |
| `4000 0000 0000 9995` | ❌ Declined |
| `4000 0025 0000 3155` | 🔐 3D Secure |

---

## 🔑 API Endpoints

### Users `/api/users`
| Method | Endpoint | Auth | Description |
|---|---|---|---|
| POST | /register | Public | Register |
| POST | /login | Public | Login |
| GET | /profile | User | Get profile |
| PUT | /profile | User | Update profile |
| POST | /wishlist/:id | User | Toggle wishlist |
| GET | / | Admin | All users |

### Products `/api/products`
| Method | Endpoint | Auth | Description |
|---|---|---|---|
| GET | / | Public | List products |
| GET | /:id | Public | Product detail |
| POST | / | Admin | Create product |
| PUT | /:id | Admin | Update product |
| DELETE | /:id | Admin | Delete product |
| POST | /:id/reviews | User | Add review |

### Orders `/api/orders`
| Method | Endpoint | Auth | Description |
|---|---|---|---|
| POST | / | User | Create order |
| GET | /myorders | User | My orders |
| POST | /:id/payment-intent | User | Stripe intent |
| PUT | /:id/pay | User | Mark as paid |
| GET | / | Admin | All orders |
| GET | /analytics | Admin | Sales analytics |

---

## 👤 Author

**Pavan R Yadav**
- GitHub: [@PAVANRYADUVANSHI](https://github.com/PAVANRYADUVANSHI)
- Email: pavanryavdavkumsi25@gmail.com
