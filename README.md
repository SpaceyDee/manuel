# Interactive UniFi Troubleshooting Manual

A dynamic, searchable, and collaborative troubleshooting guide for UniFi network environments. Designed for network professionals and support teams, this web application makes it easy to find, visualize, and contribute solutions for common (and uncommon) UniFi issues.

---

## Features

- **Powerful Search:** Find troubleshooting steps by symptom, cause, or solution.
- **Category Filtering:** Filter issues by Wi-Fi, Controller, Hardware, Configuration, Applications, Firmware, ISP/External, Multi-Site, and more.
- **Data Visualization:** See issue distribution by category via an interactive Chart.js chart.
- **Issue Details:** Click any issue for a full modal with symptom, cause, and solution breakdown.
- **Add New Issues:** Quickly contribute new troubleshooting scenarios through a guided modal form.
- **Live Collaboration:** Issues are stored and synced in Firebase Firestore for real-time updates across all users.
- **Responsive UI:** Clean, mobile-friendly design using [Tailwind CSS](https://tailwindcss.com/) and [Google Fonts](https://fonts.google.com/specimen/Inter).

---

## Demo

![Screenshot of Interactive UniFi Troubleshooting Manual](screenshot.png)

---

## Getting Started

### 1. Prerequisites

- **Web Browser:** Modern browser (Chrome, Edge, Firefox, Safari).
- **Firebase Project:** [Create a Firebase project](https://console.firebase.google.com/).
- **Firestore Database:** Enable Firestore in your Firebase project.

### 2. Configuration

You need to provide your Firebase configuration and (optionally) an app ID and authentication token.  
By default, the app expects the following JavaScript variables to be set in the environment:

```js
window.__firebase_config = JSON.stringify({
  apiKey: "...",
  authDomain: "...",
  projectId: "...",
  // ... other Firebase config
});
window.__app_id = "unifi-troubleshooting-app"; // Optional, for multi-tenancy
window.__initial_auth_token = null; // Optional, for custom auth; otherwise anonymous sign-in is used
```

You can inject these via a `<script>` tag **before** the main app or set them server-side.

### 3. Usage

Simply open `index.html` in your browser. If Firestore is empty, the app seeds it with a comprehensive set of UniFi troubleshooting issues.

- **Browse or search for issues.**
- **Filter** by category using the sidebar buttons or the chart.
- **Click an issue** for detailed steps.
- **Add new issues** using the "Add Issue" button.

---

## Deployment

You can host this as a static site (e.g. GitHub Pages, Netlify, Vercel, Firebase Hosting)  
No backend is required except for [Firebase Firestore](https://firebase.google.com/docs/firestore).

---

## Technologies Used

- [Tailwind CSS](https://tailwindcss.com/) for utility-first styling.
- [Chart.js](https://www.chartjs.org/) for visualization.
- [Google Fonts - Inter](https://fonts.google.com/specimen/Inter) for typography.
- [Firebase Firestore](https://firebase.google.com/docs/firestore) for real-time data storage.
- [Firebase Auth](https://firebase.google.com/docs/auth) for (anonymous or custom token) authentication.
- Vanilla JavaScript (ES Modules).
