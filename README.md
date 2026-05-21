# 🛒 Grocery Delivery App

A full-stack MERN grocery e-commerce platform with a customer-facing storefront, an admin dashboard for inventory and order management, and a Node.js/Express backend — all connected to a MongoDB database.

![menu page](https://github.com/user-attachments/assets/dc9cfd66-828a-4ac2-8b0a-469ee4d9e216)
![signup and login page](https://github.com/user-attachments/assets/69ed8171-5ca8-460b-959c-3db3e34ab116)
![cart page](https://github.com/user-attachments/assets/fda29103-abea-4947-9ef9-309068e7354a)

---

## Features

- User sign-up, login, and JWT-based authentication
- Browse grocery products by category
- Add to cart, manage quantities, and place orders
- Real-time order tracking and status updates
- Admin panel to add/remove products and manage orders
- Responsive UI for both desktop and mobile

---

## Tech Stack

**Frontend:** React.js, CSS  
**Backend:** Node.js, Express.js, REST APIs  
**Database:** MongoDB (Mongoose)  
**Auth:** JSON Web Tokens (JWT)  
**Payments:** Stripe  
**Tools:** Git, GitHub, VS Code, Postman

---

## Project Structure

```
grocery-delivery-app/
├── Backend/        # Express server, REST APIs, MongoDB models
├── frontend/       # React customer storefront
└── admin/          # React admin dashboard
```

---

## Getting Started

### Prerequisites
- Node.js installed
- MongoDB (local or Atlas)

### 1. Clone the repository
```bash
git clone https://github.com/rajrais2004/grocery-delivery-app.git
cd grocery-delivery-app
```

### 2. Setup Backend
```bash
cd Backend
npm install
```

Create a `.env` file in the `Backend/` folder:
```
DB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_API_KEY=your_stripe_key
PORT=4000
```

Start the backend server:
```bash
npm run server
```

### 3. Setup Frontend
```bash
cd ../frontend
npm install
npm run dev
```

### 4. Setup Admin Panel
```bash
cd ../admin
npm install
npm run dev
```

---

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/user/register` | User registration |
| POST | `/api/user/login` | User login |
| GET | `/api/food/list` | Get all products |
| POST | `/api/cart/add` | Add item to cart |
| POST | `/api/order/place` | Place an order |
| GET | `/api/order/userorders` | Get user orders |
| GET | `/api/order/list` | Get all orders (admin) |
| POST | `/api/order/status` | Update order status (admin) |

---

## Screenshots

![admin add items](https://github.com/user-attachments/assets/5574bce3-f85b-45f7-9903-7cf4ac295975)
![admin list](https://github.com/user-attachments/assets/ec39d64a-0b83-4749-9007-4ae92ffa5019)
![screenshot](https://github.com/user-attachments/assets/04ce1c2b-4b12-4be7-a6a7-db9d8841136c)

---

## License

MIT License
