# 🌐 Horizon - Fintech Banking App

A modern banking SaaS platform built with Next.js that connects multiple bank accounts, shows real-time transactions, and enables fund transfers.

---

## 📌 Introduction

Horizon is a financial application that allows users to:

* Connect multiple bank accounts
* View transactions in real time
* Transfer money between users
* Manage finances in one place

---

## ⚙️ Tech Stack

* Next.js
* TypeScript
* Appwrite
* Plaid
* Dwolla
* React Hook Form
* Zod
* Tailwind CSS
* Chart.js
* ShadCN UI

---

## 🔋 Features

* **Authentication** → Secure login system
* **Connect Banks** → Link multiple accounts using Plaid
* **Dashboard** → Total balance + recent transactions
* **My Banks** → View all connected banks
* **Transaction History** → Filter & paginate transactions
* **Real-time Updates** → Instant data updates
* **Funds Transfer** → Send money using Dwolla
* **Responsive Design** → Works on all devices

---

## 🚀 Quick Start

### Prerequisites

* Node.js
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

### Environment Variables

Create `.env` file and add:

```env
# NEXT
NEXT_PUBLIC_SITE_URL=

# APPWRITE
NEXT_PUBLIC_APPWRITE_ENDPOINT=https://cloud.appwrite.io/v1
NEXT_PUBLIC_APPWRITE_PROJECT=
APPWRITE_DATABASE_ID=
APPWRITE_USER_COLLECTION_ID=
APPWRITE_BANK_COLLECTION_ID=
APPWRITE_TRANSACTION_COLLECTION_ID=
APPWRITE_SECRET=

# PLAID
PLAID_CLIENT_ID=
PLAID_SECRET=
PLAID_ENV=sandbox
PLAID_PRODUCTS=auth,transactions,identity
PLAID_COUNTRY_CODES=US,CA

# DWOLLA
DWOLLA_KEY=
DWOLLA_SECRET=
DWOLLA_BASE_URL=https://api-sandbox.dwolla.com
DWOLLA_ENV=sandbox
```

---

### Run the Project

```bash
npm run dev
```

Open: **[http://localhost:3000](http://localhost:3000)**

---

## 📂 Project Structure

```
/app        → Pages & routing  
/components → UI components  
/lib        → API & backend logic  
/public     → Images/assets  
/types      → TypeScript types  
```

---

## 🎥 Tutorial

You can learn this project step-by-step on YouTube (JavaScript Mastery channel).

---

## 📦 Extra

* Supports clean architecture
* Reusable components
* Scalable backend structure

---

## 🚀 Conclusion

This project is a **complete fintech application** that demonstrates:

* Full-stack development
* API integration (Plaid + Dwolla)
* Secure authentication
* Real-time financial data handling

---

