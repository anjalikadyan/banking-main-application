# 🌐 Horizon - Fintech Banking Platform

Horizon is a modern financial SaaS platform that connects multiple bank accounts, displays real-time transactions, and enables peer-to-peer fund transfers.

---

## 🚀 How it Works

This application uses a powerful tech stack to provide a secure and seamless banking experience:

* **Frontend**: Next.js 14 with TypeScript and Tailwind CSS
* **Authentication & Backend**: Appwrite (handles authentication and database)
* **Banking API**: Plaid (connects to real financial institutions)
* **Payment Processing**: Dwolla (handles ACH transfers between users)
* **Visuals**: Chart.js (used for transaction and spending charts)

---

## 🛠️ How to Run the App

### Prerequisites

* Node.js (v18 or higher)
* npm
* Git

---

### Installation

```bash
git clone https://github.com/anjalikadyan/banking-main-application
cd banking
npm install
```

---

### Run the Application

**Development Mode**

```bash
npm run dev
```

Open: [http://localhost:3000](http://localhost:3000)

**Production Build**

```bash
npm run build
```

**Start Production Server**

```bash
npm start
```

---

## 🔒 Environment Variables (Important)

This project uses environment variables to store sensitive data.
<!-- 
### 1. Create Environment File

```bash
cp .env.example .env.local
```

---

### 2. Add Your Credentials

Edit `.env.local` and add:

* **Appwrite**

  * Project ID
  * API Key
  * Database ID

* **Plaid**

  * Client ID
  * Secret
  * Use sandbox for testing

* **Dwolla**

  * Key
  * Secret

---

### 3. Safety Tips

* Never upload `.env.local` to GitHub
* Keep `.env.local` in `.gitignore`
* Use sandbox keys for development
* Rotate keys if exposed

--- -->

## 📂 Project Structure

```
/app        → Pages and layouts  
/components → Reusable UI components  
/lib        → APIs, server actions, utilities  
/public     → Images and static files  
/types      → TypeScript types  
```

---
