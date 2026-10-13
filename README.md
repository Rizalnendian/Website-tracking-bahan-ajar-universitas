# Website-tracking-bahan-ajar-universitas 📚

SITTA (Sistem Informasi Tiras dan Transaksi Bahan Ajar) is a web application designed for Universitas Terbuka (UT) to manage the ordering, distribution, and tracking of study materials for its regional branches (UT-Daerah).

This system provides a centralized platform for UT-Daerah to handle their inventory of printed teaching materials (BMP), track shipments, and monitor the progress of delivery orders.

## Badges 🛡️

| Badge | Status |
|---|---||
| Primary Language | HTML |
| Stars | ★ 1 |
| Forks | 0 |

## Description 📝

SITTA serves as a comprehensive management system for the distribution of educational materials at Universitas Terbuka. It caters to UT-Daerah for managing their stock of printed teaching materials (BMP), creating and tracking delivery orders (DO), and monitoring the overall distribution process. The system aims to streamline inventory management, reduce stockouts, and provide transparency in the delivery of study materials.

## Table of Contents 📖

- [Project Title](#website-tracking-bahan-ajar-universitas-📚)
- [Badges](#badges-🛡️)
- [Description](#description-📝)
- [Table of Contents](#table-of-contents-📖)
- [Features](#features-✨)
- [Tech Stack](#tech-stack-💻)
- [Installation](#installation-⚙️)
- [Usage](#usage-🚀)
- [Project Structure](#project-structure-📁)
- [Contributing](#contributing-🤝)
- [License](#license-📄)
- [Important Links](#important-links-🔗)
- [Footer](#footer-❤️)

## Features ✨

*   **User Authentication:** Secure login system for UT-Daerah administrators with email and password validation.
*   **Inventory Management:** Detailed tracking of printed teaching materials (BMP), including code, title, category, stock quantity, price, and safety stock levels.
*   **Stock Alerts:** Visual indicators and filtering for low stock or out-of-stock items, prompting reordering.
*   **Delivery Order (DO) Creation:** Functionality to create new delivery orders with student details, selected course packages, and shipping information.
*   **Shipment Tracking:** Real-time tracking of delivery orders, including detailed trip history and status updates.
*   **Reporting and Monitoring:** Dashboards providing overviews of key metrics such as total stock, active delivery orders, shipments in progress, and recent transactions.
*   **User Roles:** Differentiated access and roles (though only Administrator role is explicitly visible in the code provided).
*   **Demo Account:** Easy access for testing with provided demo credentials.
*   **Responsive Design:** User interfaces designed to be accessible across various devices.

## Tech Stack 💻

*   **Frontend:** HTML, CSS, JavaScript, Vue.js (Vue 2.6.14)
*   **Styling:** Custom CSS with CSS Variables for theming and responsiveness.
*   **Data Management:** Client-side data simulation using JavaScript arrays (e.g., `dataBahanAjar`, `dataTracking`).
*   **Frameworks/Libraries:** Vue.js

## Installation ⚙️

This project appears to be a client-side web application. No complex installation process is required. To run the application:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Rizalnendian/Website-tracking-bahan-ajar-universitas.git
    cd Website-tracking-bahan-ajar-universitas
    ```
2.  **Open the entry point file in your web browser:**
    The primary entry point for the application is `index.html` (for login) or directly access `dashboard.html`, `stok.html`, or `tracking.html` after logging in. You can simply open these HTML files using a web browser.

**Dependencies:**
*   No explicit external dependencies like npm packages are managed via a package manager. The project relies on CDN for Vue.js.
*   Data is simulated using local JavaScript files (`js/data.js`).

## Usage 🚀

This application is designed for administrators at Universitas Terbuka regional branches (UT-Daerah) to manage the distribution of study materials.

### Login Page (`index.html`)

1.  Navigate to `index.html`.
2.  Enter your registered email and password.
3.  A demo account is provided for testing:
    *   Email: `admin@ut.ac.id`
    *   Password: `admin123`
4.  Click the 'Masuk' button.

### Dashboard (`dashboard.html`)

After successful login, you will be redirected to the dashboard, which provides:
*   A personalized greeting.
*   A summary of key metrics:
    *   Total Types of Teaching Materials 📦
    *   Active Delivery Orders 📋
    *   Shipments In Progress 🚚
    *   Low Stock Items ⚠️
*   Quick links to other sections: 'Informasi Bahan Ajar', 'Tracking Pengiriman', and 'Histori Transaksi'.
*   A table displaying the five most recent Delivery Orders.

### Inventory Management (`stok.html`)

*   View a list of all available teaching materials.
*   Filter and sort the inventory by UPBJJ (regional branch), category, and other criteria.
*   Identify items needing reorder (stock below safety level).
*   Add new bahan ajar items to the inventory.
*   Edit existing stock quantities.
*   Delete items from the inventory.

### Tracking Pengiriman (`tracking.html`)

*   Create new delivery orders by filling in student details, selecting a course package, and specifying the expedition and destination.
*   Search for existing delivery orders by their number (No. DO).
*   View the detailed tracking history of a specific delivery order, including its status and shipment progress.
*   See a list of all registered delivery orders.

### Reporting Sections (accessible from Dashboard)

*   **Monitoring Progress DO:** View the progress and status of ongoing delivery orders.
*   **Rekap Bahan Ajar:** Review monthly summaries of study material distribution.
*   **Histori Transaksi:** Access a complete history of all delivery order transactions.

## Project Structure 📁

```
Website-tracking-bahan-ajar-universitas/
├── css/
│   └── style.css
├── js/
│   ├── data.js
│   ├── script.js
│   ├── stok-app.js
│   └── tracking-app.js
├── dashboard.html
├── index.html
├── README.md
├── stok.html
└── tracking.html
```

*   **`css/`**: Contains the main stylesheet (`style.css`) for the application's UI.
*   **`js/`**: Houses JavaScript files for application logic:
    *   `data.js`: Contains sample data for materials, tracking, users, etc.
    *   `script.js`: Handles some login-related functionalities (though `index.html` now uses Vue).
    *   `stok-app.js`: Manages the stock inventory features.
    *   `tracking-app.js`: Handles delivery order creation and tracking functionalities.
*   **HTML files**: Serve as the entry points and views for different sections of the application:
    *   `index.html`: Login page.
    *   `dashboard.html`: Main dashboard view.
    *   `stok.html`: Inventory management page.
    *   `tracking.html`: Delivery order and tracking page.
*   **`README.md`**: Project documentation.

## Installation ⚙️

No explicit installation is required as this is a client-side web application. Simply clone the repository and open the HTML files in a web browser.

## Usage 🚀

See the [Usage](#usage-🚀) section above for detailed instructions on how to use the application.

## How to use 🤔

Refer to the [Usage](#usage-🚀) section for detailed operational instructions.

## API Reference 🌐

This project does not expose a public API. All data is managed client-side using JavaScript variables and simulated data within `js/data.js`.

## Contributing 🤝

As this repository has only one star and no clear contribution guidelines, we follow standard open-source practices:

1.  **Fork the repository** on GitHub.
2.  **Create a new branch** for your feature or bug fix (`git checkout -b feature/your-feature`).
3.  **Make your changes** and commit them (`git commit -m 'Add some feature'`).
4.  **Push to the branch** (`git push origin feature/your-feature`).
5.  **Open a Pull Request** on GitHub.

Please ensure your code follows the existing coding style and contributes positively to the project.

## License 📄

No license information was provided in the repository. It is assumed to be proprietary or under a default, unspecified license.

## Important Links 🔗

*   **Repository:** [Website-tracking-bahan-ajar-universitas](https://github.com/Rizalnendian/Website-tracking-bahan-ajar-universitas)
*   **Live Demo:** Not explicitly provided.

## Footer ❤️

---

**Project:** Website-tracking-bahan-ajar-universitas

**URL:** [https://github.com/Rizalnendian/Website-tracking-bahan-ajar-universitas](https://github.com/Rizalnendian/Website-tracking-bahan-ajar-universitas)

**Author:** Rizalnendian

**Contact:** [Rizalnendian's GitHub Profile](https://github.com/Rizalnendian)

--- 

[![Fork me on GitHub](https://img.shields.io/badge/github-fork-blue.svg?style=flat&logo=github)](https://github.com/Rizalnendian/Website-tracking-bahan-ajar-universitas/fork)
[![Star me on GitHub](https://img.shields.io/github/stars/Rizalnendian/Website-tracking-bahan-ajar-universitas?style=flat&logo=github)](https://github.com/Rizalnendian/Website-tracking-bahan-ajar-universitas/stargazers)
[![Issue Count](https://img.shields.io/github/issues/Rizalnendian/Website-tracking-bahan-ajar-universitas)](https://github.com/Rizalnendian/Website-tracking-bahan-ajar-universitas/issues)

---

---
**<p align="center">Generated by [ReadmeCodeGen](https://www.readmecodegen.com/)</p>**