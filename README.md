🩸 A **full-stack web application** designed to **streamline** the process of **blood donation, requests, and inventory management** for blood banks and users. Saving lives, efficiently.

---

## ✨ About the Project

The **Blood Bank App** aims to **modernize and simplify** the critical processes involved in blood management. It provides a platform for donors to register, users to request blood, and blood banks to manage their inventory efficiently. This application intends to **bridge the gap** between those who need blood and the available resources, **ultimately saving lives**.

### ✨ Key Features

* ✅ **Donor Registration:** Secure and easy registration process for blood donors, including relevant medical information (blood type, last donation date, etc.).
* 🩸 **Blood Request Management:** Users (patients, hospitals) can easily create and track blood requests, specifying blood type and urgency.
* 📦 **Inventory Management:** Blood banks can manage their stock levels, track expiry dates, and update availability in real-time.
* 🔗 **Matching System:** Intelligent system to match blood requests with available donors and inventory.
* 🔔 **Notifications:** Real-time notifications for donors about upcoming drives or urgent requests, and for requesters about the status of their request.
* 📊 **Admin Dashboard:** Comprehensive dashboard for administrators to manage users, blood banks, system settings, and generate reports.
* 📈 **Reporting and Analytics:** Generation of reports on donation trends, blood usage, and inventory levels.
* 🔒 **User Authentication and Authorization:** Secure role-based access control for different user types (donors, requesters, blood bank staff, administrators).

### 💻 Tech Stack

* **Frontend:** React, Material UI, HTML, CSS, JavaScript
* **Backend:** Node.js, Express.js, Sequelize
* **Database:** PostgreSQL
* **Other:** Docker

---

## 🚀 Getting Started

Follow these steps to get the project running on your local machine.

### ⚙️ Prerequisites

Make sure you have the following installed:

* [Node.js (version >= 16)](https://nodejs.org/en/)
* [npm (version >= 8)](https://www.npmjs.com/) or [yarn (version >= 1.22)](https://yarnpkg.com/)
* [PostgreSQL (version >= 13)](https://www.postgresql.org/)
* [Docker](https://www.docker.com/) (Optional, for containerization)

### 💾 Installation

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/KshitijaUrmale/Blood-Bank-APP.git](https://github.com/KshitijaUrmale/Blood-Bank-APP.git)
    cd Blood-Bank-APP
    ```

2.  **Install frontend dependencies:**

    ```bash
    cd client
    npm install
    ```

3.  **Install backend dependencies:**

    ```bash
    cd server
    npm install
    ```

4.  **Set up the database:**

    * Create a PostgreSQL database named `blood_bank`.
    * Create a user `blood_bank_user` with the password `your_password` (or choose your own).
    * Grant all privileges on the `blood_bank` database to the `blood_bank_user`.

    ```bash
    sudo su - postgres
    psql
    CREATE DATABASE blood_bank;
    CREATE USER blood_bank_user WITH PASSWORD 'your_password';
    GRANT ALL PRIVILEGES ON DATABASE blood_bank TO blood_bank_user;
    \q
    exit
    ```

### ⚙️ Configuration

1.  **Frontend configuration:**

    * Create `.env.local` in the `client` directory based on `.env.example`.

    ```
    REACT_APP_API_BASE_URL=http://localhost:5000/api
    ```

2.  **Backend configuration:**

    * Create `.env` in the `server` directory based on `.env.example`.

    ```
    DATABASE_URL=postgresql://blood_bank_user:your_password@localhost:5432/blood_bank
    PORT=5000
    JWT_SECRET=your_secret_key
    ```

    * Make sure to replace `your_password` with the actual password you set for the `blood_bank_user`.

---

## 💡 Usage

1.  **Start the PostgreSQL database:**

    * Ensure the PostgreSQL server is running.

2.  **Start the backend server:**

    ```bash
    cd server
    npm run dev
    ```

3.  **Start the frontend development server:**

    ```bash
    cd client
    npm start
    ```

### 👥 User Roles

* **Donor:** Register, update profile, view donation history, receive notifications.
* **Requester:** Create/track requests, manage history.
* **Blood Bank Staff:** Manage inventory, process requests, update availability, manage donors.
* **Administrator:** Manage users, blood banks, system settings, generate reports.

### 🔑 Key Workflows

* **Donating Blood:** Registered donors participate in drives or schedule appointments. Inventory updated by staff.
* **Requesting Blood:** Users/hospitals submit requests. System notifies blood banks/searches donors.
* **Inventory Management:** Staff adds/updates blood units, tracks expiry. System alerts for low stock/expiry.

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1.  **Fork** the repository.
2.  Create a new branch (`git checkout -b feature/enhancement`).
3.  Commit your changes (`git commit -am 'Add new feature'`).
4.  Push to the branch (`git push origin feature/enhancement`).
5.  Open a **pull request**.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.



 
