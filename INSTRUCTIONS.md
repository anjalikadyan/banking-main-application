# Horizon - Fintech Banking Platform

Horizon is a modern financial SaaS platform that connects multiple bank accounts, displays real-time transactions, and enables peer-to-peer fund transfers.

---

## 🚀 **How it Works**

This application uses a sophisticated tech stack to provide a secure and seamless banking experience:

- **Frontend**: [Next.js 14](file:///d%3A/Development/0.Projects/banking-main1/banking-main/package.json#L24) with [TypeScript](file:///d%3A/Development/0.Projects/banking-main1/banking-main/package.json#L47) and [Tailwind CSS](file:///d%3A/Development/0.Projects/banking-main1/banking-main/package.json#L46) for a responsive and performant UI.
- **Authentication & Backend**: [Appwrite](file:///d%3A/Development/0.Projects/banking-main1/banking-main/lib/appwrite.ts) handles user authentication (SSR) and database management.
- **Banking API**: [Plaid](file:///d%3A/Development/0.Projects/banking-main1/banking-main/lib/plaid.ts) connects the platform to thousands of real financial institutions.
- **Payment Processing**: [Dwolla](file:///d%3A/Development/0.Projects/banking-main1/banking-main/lib/actions/dwolla.actions.ts) facilitates secure automated clearing house (ACH) transfers between users.
- **Visuals**: [Chart.js](file:///d%3A/Development/0.Projects/banking-main1/banking-main/package.json#L14) and [DoughnutChart.tsx](file:///d%3A/Development/0.Projects/banking-main1/banking-main/components/DoughnutChart.tsx) provide data visualization for spending patterns.

---

## 🛠️ **How to Run the App**

Follow these steps to set up the project locally:

### **Prerequisites**
- [Node.js](https://nodejs.org/) (v18 or higher)
- [npm](https://www.npmjs.com/) (installed with Node.js)
- [Git](https://git-scm.com/)

### **Installation**
1.  **Clone the repository**:
    ```bash
    git clone https://github.com/adrianhajdin/banking.git
    cd banking
    ```
2.  **Install dependencies**:
    ```bash
    npm install
    ```

### **Run the Application**
1.  **Development Mode**:
    ```bash
    npm run dev
    ```
    Open [http://localhost:3000](http://localhost:3000) in your browser.
2.  **Production Build**:
    ```bash
    npm run build
    ```
3.  **Start Production Server**:
    ```bash
    npm start
    ```

---

## 🔒 **How to Change Private Settings Safely**

The application uses **Environment Variables** to store sensitive information like API keys. **Never** commit your `.env` files to version control.

### **1. Create your Local Environment File**
Copy the template from [.env.example](file:///d%3A/Development/0.Projects/banking-main1/banking-main/.env.example) to a new file named `.env.local`:
```bash
cp .env.example .env.local
```

### **2. Configure the Variables**
Open [.env.local](file:///d%3A/Development/0.Projects/banking-main1/banking-main/.env.local) and add your credentials:

- **Appwrite**: Create a project on [Appwrite Cloud](https://cloud.appwrite.io/) and get your `Project ID`, `API Key`, and `Database IDs`.
- **Plaid**: Sign up at [Plaid Dashboard](https://dashboard.plaid.com/) and get your `Client ID` and `Secret`. Use `sandbox` for testing.
- **Dwolla**: Register at [Dwolla Sandbox](https://dashboard-sandbox.dwolla.com/) to get your `Key` and `Secret`.

### **3. Safety Best Practices**
- **.gitignore**: Ensure `.env.local` is listed in your [.gitignore](file:///d%3A/Development/0.Projects/banking-main1/banking-main/.gitignore) file (it is by default).
- **Environment Separation**: Use different keys for development (sandbox) and production environments.
- **Rotate Secrets**: If you suspect a key has been leaked, rotate (replace) it immediately in your service dashboard.

---

## 📂 **Project Structure**

- `/app`: Next.js App Router pages and layouts.
- `/components`: Reusable UI components (Sidebar, AuthForm, BankCard, etc.).
- `/lib`: Server actions, API configurations, and utility functions.
- `/public`: Static assets like icons and images.
- `/types`: TypeScript interface and type definitions.
