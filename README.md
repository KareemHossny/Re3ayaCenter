# Re3aya Center – Full Hospital Appointment System

![React](https://img.shields.io/badge/Frontend-React_19-blue)
![Node](https://img.shields.io/badge/Backend-Node.js-green)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-brightgreen)
![JWT](https://img.shields.io/badge/Auth-JWT-orange)
![OAuth](https://img.shields.io/badge/Auth-Google_OAuth-red)
![Cloudinary](https://img.shields.io/badge/Storage-Cloudinary-blueviolet)
![Vercel](https://img.shields.io/badge/Deployment-Vercel-black)
![Production](https://img.shields.io/badge/Status-Production-green)

**Re3aya** is a **production-ready full-stack hospital appointment management system**.  
It provides **role-based dashboards** for Patients, Doctors, and Admins, **secure appointment scheduling**, specialization management, and real-time workflow coordination.  

Designed for real-world usage with **scalable REST APIs**, **JWT & Google OAuth authentication**, and **role-based access control (RBAC)**.

---

## 🚀 Live Demo (Fully Functional)

- **Frontend:** [https://re3aya-center.vercel.app](https://re3aya-center.vercel.app)  
- **Backend API:** [https://re3aya-backend.vercel.app/api](https://re3aya-backend.vercel.app/api)

> The system is fully operational: Patients can book appointments, Doctors can manage schedules and prescriptions, and Admins can manage users and specializations.

---

## 📦 Source Code

- **Frontend Repository:** [Re3aya-Frontend](https://github.com/KareemHossny/Re3aya-Frontend)  
- **Backend Repository:** [Re3aya-Backend](https://github.com/KareemHossny/Re3aya-Backend)

---

## 🧠 System Architecture

```
Patient / Doctor / Admin
          ↓
Frontend (React, role dashboards)
          ↓
Backend API (Express + JWT + RBAC)
          ↓
MongoDB Database
```

**Highlights:**

- Role-based dashboards for Patients, Doctors, and Admins  
- REST API with JWT authentication & Google OAuth  
- MongoDB relational references: User, Appointment, Specialization, DoctorSchedule  
- Cloudinary for media storage  
- Secure image uploads & access control

---

## 🔐 Authentication & Security

- JWT Bearer token + Google OAuth  
- Role-based access control enforced by middleware (`protect`, `authorize`)  
- Password hashing with bcryptjs  
- API rate limiting on sensitive routes  
- HTTP Parameter Pollution (hpp) protection  
- CORS allowlist  
- Unique appointment index to prevent double bookings  
- Frontend session persisted with secure localStorage token  

> All security and auth flows are fully operational in the deployed demo.

---

## ✨ Core Features (Fully Working)

### 🌍 Public Access
- Browse doctors & specializations  
- View doctor details and public platform statistics

### 👤 Patient Dashboard
- Search/filter doctors  
- Book & cancel appointments  
- View personal appointment statistics

### 👨‍⚕️ Doctor Dashboard
- Manage profile & schedule  
- View appointments  
- Cancel/complete appointments  
- Create structured prescription notes  
- View performance statistics

### 🛠 Admin Dashboard
- Manage users & role assignments  
- Create/edit/delete specializations  
- Upload/delete specialization images  
- View system-level stats

> All features are fully implemented and functional in the live demo.

---

## 🏗 Design Decisions

- Role-based routing for maintainability  
- Centralized Axios client with interceptors  
- Cloudinary storage for scalable media management  
- Appointment conflict prevention with unique DB index  
- Frontend localization (Arabic/English) via i18next  
- Production-ready deployment with Vercel (Frontend + Backend)  

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repositories

```bash
# Frontend
git clone https://github.com/KareemHossny/Re3aya-Frontend.git

# Backend
git clone https://github.com/KareemHossny/Re3aya-Backend.git
```

### 2️⃣ Frontend Setup

```bash
cd Re3aya-Frontend
npm install
npm start
```

**Environment variables (`.env`):**

```
REACT_APP_API_URL=https://re3aya-backend.vercel.app/api
REACT_APP_GOOGLE_CLIENT_ID=<your_google_client_id>
```

### 3️⃣ Backend Setup

```bash
cd Re3aya-Backend
npm install
npm run dev
```

**Backend `.env`:**

```
PORT=5000
NODE_ENV=development
MONGO_URI=<your_mongo_uri>
JWT_SECRET=<your_jwt_secret>
JWT_EXPIRE=7d
GOOGLE_CLIENT_ID=<your_google_client_id>
CLOUDINARY_CLOUD_NAME=<your_cloud_name>
CLOUDINARY_API_KEY=<your_api_key>
CLOUDINARY_API_SECRET=<your_api_secret>
ADMIN_EMAIL=<admin_email>
ADMIN_PASSWORD=<your_admin_password>
```

---

## 🔄 Real-World Workflow Example

1. **Patient:** Browses doctors → selects specialization → books appointment  
2. **Doctor:** Views schedule → confirms or cancels appointments → adds prescription notes  
3. **Admin:** Manages users and specializations → monitors platform statistics

> This workflow demonstrates fully integrated frontend + backend functionality, identical to a live production system.

---

## 🧪 Future Improvements

- Migrate hardcoded frontend configs to environment variables  
- Add automated backend tests (unit/integration/e2e)  
- OpenAPI / Swagger API documentation  
- Structured logging & monitoring  
- Refresh token lifecycle for stronger session management

---

## 👨‍💻 Author

**Kareem Hossny** – Full Stack MERN Developer  
Open to freelance & junior full-stack opportunities

---
