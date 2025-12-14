## MERN Bookstore — Full-Stack Application

A complete Bookstore web application built using the MERN stack, supporting Users, Sellers, and Admins with features like book management, orders, reviews, authentication, PDF generation, dashboards, and more.

## 🚀 Live Features
### 👤 User Features

Signup / Login / Logout

Browse books by category, search, rating

Add to Cart

Buy Now & Checkout

Order history

Download Order Invoice (PDF)

Add book reviews (with rating stars)

View average book rating

Profile update (avatar upload, phone update)

## 🛍️ Seller Features

Seller Dashboard (Revenue, Stock, Books, Orders)

Add Book (with cover image + PDF upload)

Edit Book

Manage Books

View Seller Orders

Fetch Buyer details for each order

## 🛠️ Admin Features

Admin Dashboard (Users, Books, Orders, Sellers count)

View all Users

View all Books

View all Orders

View Seller List

Navigate to all management pages

System-wide monitoring

## ⭐ Other Key Features

PDF invoice generation

Printing UI

Category cards with average rating

Modern UI with Bootstrap + custom styles

Authentication sync across tabs

Role-based navbar (User / Seller / Admin / Guest)


## 🧰 Tech Stack
Layer	Technology
Frontend	React + React Router DOM + Bootstrap
Backend	Node.js, Express.js
Database	MongoDB + Mongoose
Authentication	JWT
File Uploads	Multer
PDF Generation	pdf-lib / html-pdf / pdfkit (your implementation)
Notifications	React Toastify


## 📂 Project Structure
Bookstore/
│── Backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── uploads/ (images, pdfs)
│   ├── server.js
│   └── .env
│
│── Frientend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── api.js
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
│
│── README.md


## 🔑 Important API Endpoints
# 📘 Books
Method	Endpoint	Description
GET	/item	Get all books
GET	/item/:id	Book details
POST	/item	Add Book (Seller/Admin)
PUT	/item/:id	Edit Book
DELETE	/item/:id	Delete Book

# 👤 Auth
Method	Endpoint	Role
POST	/signup	User
POST	/login	User
POST	/slogin	Seller
POST	/alogin	Admin


# ⭐ Reviews
Method	Endpoint	Description
POST	/item/:id/review	Submit review & rating

# 🛒 Orders
Method	Endpoint	Description
POST	/userorder	Place order
GET	/orders	Admin: all orders
GET	/order/:id	View order
GET	/order/:id/pdf	Download PDF
