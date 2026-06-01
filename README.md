# ShopNow — eCommerce App 🛒

Amazon-like full-stack eCommerce platform with JWT auth, Stripe payments, product reviews, wishlist, admin dashboard, and Cloudinary image uploads.

## 🚀 Features
- JWT Authentication (register / login / protected routes)
- Product listing with search, category filter, price range, sort
- Product detail with image gallery and reviews
- Star ratings (1–5) by logged-in users
- Shopping cart with localStorage persistence
- Checkout with Stripe payment
- Order tracking with status steps
- User profile with shipping address
- Wishlist toggle
- Admin dashboard with sales analytics
- Admin CRUD for products, orders, users
- Image upload via Cloudinary
- Pagination on products and orders
- Responsive mobile + desktop UI
- Docker Compose for full-stack deployment

## 🛠️ Tech Stack
- **Frontend:** Next.js, Redux, Tailwind CSS
- **Backend:** Node.js, Express
- **Database:** MongoDB
- **Payments:** Stripe
- **Storage:** Cloudinary

## ⚡ Quick Start

### Backend
```bash
cd backend
npm install
cp .env.example .env
npm run dev
```

### Frontend
```bash
cd frontend
npm install
cp .env.local.example .env.local
npm run dev
```

## 💳 Stripe Test Cards
| Card Number | Scenario |
|---|---|
| 4242 4242 4242 4242 | Success |
| 4000 0000 0000 9995 | Declined |

## 👤 Author
**Pavan R Yadav**
- GitHub: [@PAVANRYADUVANSHI](https://github.com/PAVANRYADUVANSHI)
