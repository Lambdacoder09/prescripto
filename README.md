<div align="center">
  
# PRESCRIPTO 👨‍⚕️🏥🤒
</div>

This full stack appointment booking system can be used by a doctor or a hospital. Because in this project I have created 3 level of authentication. 1st one is for Patients, so that patient can login on the website, book appointment with doctor and manage the booked appointment. 2nd one is doctor login, so that doctor can login and check the appointment and their earning. Doctor can update their profile also from dashboard. 3rd one is Admin Dashboard where admin can manages the appointment and admin can also manage the doctor profile.

<br/><hr/><br/>

<div align="center">

## LIVE - DEMO 🌐
  
**UI** 👉 [LINK](https://prescripto-frontend-lovat.vercel.app)

**Admin Dashboard** 👉 [LINK](https://prescripto-admin-beta.vercel.app)
</div>

<br/><hr/><br/>

## 🚀 Getting Started

Follow these instructions to set up and run the Prescripto project locally.

### 📋 Prerequisites

Before you begin, ensure you have the following installed:
- **Node.js** (v14 or higher) - [Download here](https://nodejs.org/)
- **MongoDB** - [Download here](https://www.mongodb.com/try/download/community) or use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) (cloud database)
- **npm** (comes with Node.js)

### 📦 Installation

#### 1. Clone the Repository
```bash
git clone https://github.com/elyse502/prescripto.git
cd prescripto
```

#### 2. Backend Setup
```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory with the following variables:
```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_admin_password
CLOUDINARY_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key
```

> **Note**: Replace the placeholder values with your actual credentials.

#### 3. Admin Panel Setup
```bash
cd ../admin
npm install
```

Create a `.env` file in the `admin` directory:
```env
VITE_BACKEND_URL=http://localhost:4000
```

#### 4. Frontend (Clientside) Setup
```bash
cd ../clientside
npm install
```

Create a `.env` file in the `clientside` directory:
```env
VITE_BACKEND_URL=http://localhost:4000
```

### ▶️ Running the Application

You need to run all three components simultaneously in separate terminal windows:

#### Terminal 1 - Backend Server
```bash
cd backend
npm run server
```
The backend will start on `http://localhost:4000`

#### Terminal 2 - Admin Panel
```bash
cd admin
npm run dev
```
The admin panel will be available at the URL shown in the terminal (typically `http://localhost:5173`)

#### Terminal 3 - Frontend (User Interface)
```bash
cd clientside
npm run dev
```
The frontend will be available at the URL shown in the terminal (typically `http://localhost:5174`)

### 🎯 Access Points

Once all services are running:
- **Frontend (User)**: Visit the URL shown in Terminal 3
- **Admin Dashboard**: Visit the URL shown in Terminal 2
- **Backend API**: `http://localhost:4000`

<br/><hr/><br/>

<div align="center">

# User Dashboard 👤:
![UI](https://github.com/user-attachments/assets/f953ae81-7cc8-4b6b-8101-c3aa47d0aada)

<br /><hr /><br />

# Doctor Panel 🧑‍⚕️:
![doctor-panel](https://github.com/user-attachments/assets/ed488e0a-a61a-4cb1-b95a-f19b9135f9b2)

<br /><hr /><br />

# Admin Panel 🎯:
![admin-panel](https://github.com/user-attachments/assets/5479b3c0-0663-41ec-9fe2-17434249155c)

</div>

<br/><hr/><br/>

## 🚀 Deployment Guide (Vercel)

This project is configured for easy deployment to **Vercel**. Since it contains three distinct components (Backend, Admin, and Frontend), you should deploy them as separate projects or use Vercel's monorepo support.

### 1. Backend Deployment
1. Go to the [Vercel Dashboard](https://vercel.com/dashboard) and click **"Add New" > "Project"**.
2. Import your GitHub repository.
3. In the **"Framework Preset"**, select `Other`.
4. Set the **Root Directory** to `backend`.
5. Add the following **Environment Variables**:
   - `MONGODB_URI` (Your MongoDB connection string)
   - `JWT_SECRET` (A secure random string)
   - `ADMIN_EMAIL` (For admin dashboard login)
   - `ADMIN_PASSWORD` (For admin dashboard login)
   - `CLOUDINARY_NAME`
   - `CLOUDINARY_API_KEY`
   - `CLOUDINARY_SECRET_KEY`
6. Click **Deploy**. Once finished, copy the **Deployment URL** (e.g., `https://prescripto-backend.vercel.app`).

### 2. Admin Panel Deployment
1. Click **"Add New" > "Project"** again and select the same repository.
2. In the **"Framework Preset"**, select `Vite`.
3. Set the **Root Directory** to `admin`.
4. Add the following **Environment Variable**:
   - `VITE_BACKEND_URL`: (Paste your backend deployment URL from step 1)
5. Click **Deploy**.

### 3. Frontend (Clientside) Deployment
1. Click **"Add New" > "Project"** again and select the same repository.
2. In the **"Framework Preset"**, select `Vite`.
3. Set the **Root Directory** to `clientside`.
4. Add the following **Environment Variable**:
   - `VITE_BACKEND_URL`: (Paste your backend deployment URL from step 1)
5. Click **Deploy**.

> [!TIP]
> Make sure your MongoDB Atlas (or other provider) allows connections from any IP address (`0.0.0.0/0`) since Vercel's deployment IPs are dynamic.

<br/><hr/><br/>

## Author :black_nib:
- _[NIYIBIZI Elysée](https://linktr.ee/niyibizi_elysee)👨🏿‍💻 | [Github](https://github.com/elyse502) | [Linkedin](https://www.linkedin.com/in/niyibizi-elys%C3%A9e/) | [Twitter](https://twitter.com/Niyibizi_Elyse)._

<!--I'm [Elysée NIYIBIZI](https://elyseeniyibizi.me/) 👋

A **super passionate** Rwandan **software engineer** 🤗 And a true cheese 🧀 & chocolate 🍫 lover! 😋 You can reach me at _hi {[AT]} elyseeniyibizi [{D0T}] me_ -->

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/niyibizi-elys%C3%A9e/) [![@phenrysay](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/Niyibizi_Elyse) [![pH-7](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/elyse502)

<br /><hr /><br />

## License 📝

This project is distributed under [MIT license](https://github.com/elyse502/prescripto/blob/main/LICENSE). Enjoy! 🎉

<br /><br />




