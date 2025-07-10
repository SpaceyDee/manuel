# Interactive IT Troubleshooting Manual

A dynamic, searchable, and collaborative troubleshooting guide for multiple IT products. Designed for IT professionals and support teams, this web application makes it easy to find, visualize, and contribute solutions for common (and uncommon) issues across various products including UniFi networking equipment and Microsoft 365.

---

## Features

- **Powerful Search:** Find troubleshooting steps by symptom, cause, or solution.
- **Product Filtering:** Filter issues by product (UniFi, Microsoft 365, and more).
- **Category Filtering:** Filter issues by product-specific categories (e.g., Wi-Fi, Email, Teams, SharePoint).
- **Data Visualization:** See issue distribution by category via an interactive Chart.js chart.
- **Issue Details:** Click any issue for a full modal with symptom, cause, and solution breakdown.
- **Add New Issues:** Quickly contribute new troubleshooting scenarios for any product through a guided modal form.
- **Session-Based Storage:** Issues are stored for the current session (no backend database required).
- **Responsive UI:** Clean, mobile-friendly design using [Tailwind CSS](https://tailwindcss.com/) and [Google Fonts](https://fonts.google.com/specimen/Inter).

---

## Demo

![Screenshot of Interactive IT Troubleshooting Manual](screenshot.png)

---

## Getting Started

### Prerequisites

- **Web Browser:** Modern browser (Chrome, Edge, Firefox, Safari).

### Usage

Simply open `index.html` in your browser. The app comes pre-loaded with troubleshooting issues for:

- **UniFi networking equipment** (Wi-Fi, Controller, Hardware, etc.)
- **Microsoft 365** (Email, Account, Teams, SharePoint, Office Apps)

- **Browse or search for issues** across all products.
- **Filter by product** to focus on specific technologies (UniFi, Microsoft 365, etc.).
- **Filter by category** within a product using the sidebar buttons or the chart.
- **Click an issue** for detailed troubleshooting steps.
- **Add new issues** for any product using the "Add Issue" button.

---

## Deployment

You can host this as a static site on any platform (e.g., GitHub Pages, Netlify, Vercel)  
No backend is required as all data is stored in the frontend and persisted only for the current session.

---

## Technologies Used

- [Tailwind CSS](https://tailwindcss.com/) for utility-first styling.
- [Chart.js](https://www.chartjs.org/) for data visualization.
- [Google Fonts - Inter](https://fonts.google.com/specimen/Inter) for typography.
- Vanilla JavaScript for application logic.
