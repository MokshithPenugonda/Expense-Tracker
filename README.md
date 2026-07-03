# 💸 Expense Tracker Web App

A full-stack **MERN** (MongoDB, Express.js, React + Vite, Node.js) application for tracking your income and expenses. Designed with a **modern gradient UI**, includes **JWT-based authentication**, **global state management**, and interactive data visualizations.

---

## 🚀 Features

- 🔐 User Registration & Login (JWT Auth)
- 📊 Dashboard with Analytics (Pie + Line Charts)
- ➕ Add, View, Edit & Delete Transactions
- 🗂️ Manage Custom Categories (Income/Expense)
- 📜 Transaction History with Filters
- 📤 Export data to CSV and PDF format
- 💡 Global State with React Context API
- 🎨 Gradient UI with Tailwind CSS + ShadCN UI
- ⚠️ 404 Not Found Page

---

## 🛠️ Tech Stack

### Frontend
- **React** (with Vite + TypeScript)
- **Tailwind CSS** for styling
- **ShadCN UI** components
- **React Router DOM** (routing)
- **React Hook Form + Yup** (form validation)
- **Recharts** for charts
- **react-hot-toast** (notifications)
- **jsPDF + FileSaver** (PDF/CSV export)
- **papaParse

### Backend
- **Node.js** with **Express.js**
- **MongoDB Atlas** with **Mongoose**
- **JWT** for auth
- **Bcrypt** for password hashing

---

##  Project Structure

```
Expense-Management-System/
│
├── client/                              # Frontend (React + Vite)
│   ├── public/
│   │   └── icon.png
│   ├── src/
│   │   ├── api/
│   │   │   └── axios.ts
│   │   ├── assets/
│   │   │   └── react.svg
│   │   ├── components/
│   │   │   └── Layout.tsx
│   │   ├──  context/
│   │   │   └──AuthContext.tsx
│   │   ├── pages/
│   │   │   └──AddTransaction.tsx
│   │   │   └──Auth.tsx
│   │   │   └──Category.tsx
│   │   │   └──Dashboard.tsx
│   │   │   └──Home.tsx
│   │   │   └──NotFound.tsx
│   │   │   └──TransactionHistory.tsx
│   │   ├── routes/
│   │   │   └── ProtectedRoute.tsx
│   │   ├── utils/
│   │   │   └── validationSchema.ts
│   │   ├── App.css
│   │   ├── App.tsx
│   │   ├── index.css
│   │   ├── main.tsx
│   │   └── vite-env.d.ts
│   ├── .gitignore
│   ├── eslint.config.js
│   ├── index.html
│   ├── package.json
│   ├── package-lock.json
│   ├── postcss.config.js
│   ├── tailwind.config.js
│   ├── tsconfig.json
│   ├── tsconfig.app.json
│   └── vite.config.ts         
│
├── server/                             # Backend (Node + Express)
│   ├── src/
│   │   ├── controllers/
│   │   │   └── categoryController.ts
│   │   │   └── transactionController.ts
│   │   │   └── userController.ts
│   │   ├── middleware/
│   │   │   └── authMiddleware.ts
│   │   ├── models/
│   │   │   └── Category.ts
│   │   │   └── Transaction.ts
│   │   │   └── User.ts
│   │   ├── routes/
│   │   │   └── categoryRoutes.ts
│   │   │   └── transactionRoutes.ts
│   │   │   └── userRoutes.ts
│   │   ├── utils/
│   │   │   └── createDefaultCategorles.ts
│   │   │   └── generatetoken.ts
│   │   └── index.ts
│   ├── .env
│   ├── package.json
│   ├── package-lock.json
│   └── tsconfig.json
│
└── README.md
```


 ## 🧑‍💻 Getting Started

### 1️⃣ Clone the Repo

```

cd Expense-Management-System
```

### 2️⃣ Setup Backend

```
cd server
npm install < the dependecies which we want to install >
```

Create `.env` file:

```env
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
PORT=5000
```

Start the server:

```
cd client
npm run dev
```

### 3️⃣ Setup Frontend

```
cd client
First initialize the react project with the commands then we need to run the commands which are below 
npm install
npm run dev
```

---

## 🔐 Authentication Flow

- Users register or login via `/auth`
- JWT token stored in `localStorage`
- Token is attached to every API request (via Axios interceptor)
- Protected routes (Dashboard, Add Transaction, History) are guarded

---
## 🖼️ Screenshots
 # Home page
 ![Home page](<screenshots/Screenshot 2025-07-28 194717.png>)
 # Login page
![Login page](<screenshots/Screenshot 2025-07-28 194731.png>)
 # Layout page
 ![Layout page](<screenshots/Screenshot 2025-07-28 194756.png>)
 # Dashboard page
 ![Dashboard page](<screenshots/Screenshot 2025-07-28 194811.png>)
 # Transaction History page
![Transaction History page](<screenshots/Screenshot 2025-07-28 194831.png>)

## ⚙️ Additional Features 

- ✅ Responsive UI
- 🧠 404 Page on unknown routes
- 📂 CSV Export of Transaction History



