# foodie-website
Built responsive web application with cart functionality using HTML, CSS, JavaScript.

# 🍔 Foodie. — Modern E-Commerce Culinary Experience

This project is a high-performance, responsive **Frontend Web Application** designed for the modern food delivery industry. It features a dynamic product catalog, a seamless cart management system, and a sophisticated UI/UX built with a mobile-first approach.

---

## 🎨 Architectural Overview

### 🌐 Frontend Structure (`index.html`)
The backbone of the application, utilizing semantic HTML5 to ensure accessibility and SEO optimization. 
* **Dynamic Navigation:** A sticky header providing instant access to the Menu, Services, and the interactive Cart.
* **Swiper Integration:** Implements a high-end visual slider for featured promotions.
* **Modular Layout:** Structured into logical sections: Hero, Popular Categories, Menu Grid, and a comprehensive Footer.

### 💄 Design System (`style.css`)
A professional-grade stylesheet utilizing **CSS Custom Properties (Variables)** for consistent branding and rapid scaling.
* **Brand Identity:** Uses a premium color palette featuring `Gold Finger` (#F2BD12) for calls-to-action and `Eye Ball` (#FFFDF7) for a clean, appetizing background.
* **Modern Typography:** Integrated with "Roboto Condensed" for a sleek, readable, and bold aesthetic.
* **Responsive Engine:** Employs advanced **Media Queries** and **Flexbox** layouts to ensure a flawless experience across mobile, tablet, and desktop devices.
* **Interactive Transitions:** Smooth hover effects and "slide-out" animations for cart items to enhance user feedback.

### 🧠 Logic & Interactivity (`main.js`)
The "brain" of the store, handling data-driven interactions without requiring a page reload.
* **Asynchronous Data Fetching:** Uses the **Fetch API** to consume `products.json`, simulating a real-world database interaction.
* **Cart Lifecycle Management:** * **Add/Remove Logic:** Dynamically injects items into the DOM.
    * **Quantity Controller:** Real-time mathematical updates for individual item totals and the overall cart grand total.
* **State Management:** Tracks `cartProduct` arrays to ensure data consistency during a browsing session.
* **Component Initialization:** Orchestrates the Swiper.js slider and hamburger menu toggles for mobile navigation.

### 📦 Data Layer (`products.json`)
A structured **JSON Repository** that serves as the "Single Source of Truth" for the menu.
* **Schema:** Each object contains a unique `id`, `name`, `price`, and `image` path.
* **Scalability:** Allows the menu to be updated or expanded instantly without touching the core HTML/CSS code.

---

## 🚀 Key Technical Features

| Feature | Implementation | Benefit |
| :--- | :--- | :--- |
| **Dynamic Cart** | JavaScript DOM Manipulation | Enhances UX by allowing users to shop without interruptions. |
| **Mobile-First UX** | CSS Media Queries & Hidden Sidebars | Guarantees 100% usability for users on the go. |
| **Asset Optimization** | Swiper & Deferred Scripts | Ensures fast loading times and smooth visual performance. |
| **Calculated Totals** | Real-time JS Logic | Provides immediate transparency on pricing and quantities. |

---

## 🛠️ Tech Stack
* **HTML5:** Structural Markup.
* **CSS3:** Advanced Styling (Flexbox, Variables, Animations).
* **JavaScript (ES6+):** Dynamic Functionality & State Management.
* **JSON:** Backend-style data simulation.
* **Swiper.js:** Premium touch-responsive sliders.
* **FontAwesome:** High-fidelity iconography.

---

### 💡 Execution Flow
1.  **Load:** Browser parses `index.html` and `style.css`.
2.  **Initialize:** `main.js` triggers `initApp()`.
3.  **Fetch:** Product data is pulled from `products.json` and rendered into the grid.
4.  **Interact:** User adds items to the cart; the DOM updates instantly with recalculated totals.
