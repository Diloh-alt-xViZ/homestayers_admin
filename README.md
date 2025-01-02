# Homestayers Admin Panel

The **Homestayers Admin Panel** is the administrative dashboard for managing the Homestayers platform. This panel empowers administrators to oversee and control the platform's key functionalities, ensuring smooth operations, effective user management, and system integrity.

---

## **Table of Contents**

1. [Features](#features)
2. [Tech Stack](#tech-stack)
3. [Getting Started](#getting-started)
4. [Folder Structure](#folder-structure)
5. [Usage](#usage)
6. [Contributing](#contributing)
7. [License](#license)

---

## **Features**

### **1. Dashboard**
- **Overview Cards:** Total users, active listings, completed bookings, and revenue.
- **Analytics:** Charts and insights for bookings, earnings, and user growth trends.

### **2. User Management**
- View, edit, and deactivate user accounts.
- Search and filter users by name, email, or account status.
- Manage host/guest verification status.

### **3. Listing Management**
- Approve or reject new property listings.
- View and moderate listings flagged for inappropriate content.
- Filter properties by location, host, or status.

### **4. Booking Management**
- View all bookings: active, completed, or canceled.
- Resolve disputes between guests and hosts.
- Manage booking cancellations and refunds.

### **5. Payment Tracking**
- View all transactions (host payouts and guest payments).
- Track pending and completed refunds.
- Generate revenue reports by date or category.

### **6. Review Moderation**
- Manage guest and host reviews.
- Flag or remove inappropriate reviews.

### **7. Support System**
- View and manage user-reported issues or disputes.
- Assign priority levels and track resolutions.

### **8. System Settings**
- Configure platform fees, cancellation policies, and payout settings.
- Customize email templates for notifications.
- Manage supported languages and currencies.

---

## **Tech Stack**

### **Frontend**
- **React.js**: Modern UI library for building the admin interface.
- **Material-UI**: Pre-designed components for a sleek and professional look.
- **Recharts**: Charts and data visualization for analytics.

### **Backend**
- **Springboot (Java)**: REST API for data and business logic.
- **Postgres**: Database for storing users, listings, bookings, and payments.
- **JWT**: Authentication and secure access control.

### **Hosting & Tools**
- **Railway**: For image storage and static asset delivery.
- **Paynow API**: Secure payment integration.
- **AfricasTalkingSmsApi**: Sms notification service.

---

## **Getting Started**

### **1. Prerequisites**
- Node.js (v16 or higher)
- Postgres (local or cloud-based)
- Paynow account for payments
- AWS S3 or Cloudinary for media management

### **2. Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/homestayers-admin-panel.git
   cd homestayers-admin-panel
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create an `.env` file in the root directory and configure the following variables:
   ```env
   REACT_APP_API_BASE_URL=http://localhost:5000
   REACT_APP_Paynow_PUBLIC_KEY=your_stripe_public_key
   ```

4. Start the development server:
   ```bash
   npm start
   ```

5. Access the admin panel in your browser at `http://localhost:3000`.

---

## **Folder Structure**

```plaintext
homestayers-admin-panel/
├── public/
│   ├── index.html
├── src/
│   ├── components/         # Reusable UI components
│   │   ├── Sidebar/
│   │   ├── Navbar/
│   ├── pages/              # Pages like Dashboard, Users, Listings
│   │   ├── DashboardPage.js
│   │   ├── UsersPage.js
│   │   ├── ListingsPage.js
│   ├── services/           # API service calls
│   ├── context/            # Global state management
│   ├── utils/              # Helper functions
│   ├── styles/             # Custom styling or MUI themes
│   ├── App.js
│   ├── index.js
```

---

## **Usage**

### Development
1. Start the backend API server (refer to the main Homestayers API repository).
2. Run the admin panel locally with `npm start`.

### Production
1. Build the app for production:
   ```bash
   npm run build
   ```
2. Deploy the `build/` folder to your hosting platform (e.g., AWS S3, Netlify, or Vercel).

---

## **Contributing**

We welcome contributions to improve the Homestayers Admin Panel. Please follow these steps:

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request.

---

## **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to reach out with any questions or feedback. Let's make Homestayers better together! 🚀
