# e-plantShopping 🌿

**Paradise Nursery** — A React + Redux shopping cart application for an online plant store.

---

## Overview

Paradise Nursery is a full-featured e-commerce shopping application built with React and Redux Toolkit. Users can browse a curated collection of houseplants organized by category, add them to a cart, and manage their order — all powered by a global Redux state.

---

## Features

- 🏠 **Landing Page** — Welcome screen with a "Get Started" button linking to the product listing
- 🌱 **Product Listing Page** — Plants grouped into categories, each with image, name, description, and price
- 🛒 **Shopping Cart** — Full cart management with quantity controls, item subtotals, and total cost
- 🔢 **Live Cart Count** — Cart icon in the navbar dynamically updates with total item count
- ✅ **Add to Cart UX** — Button disables and updates to "Added to Cart" after a plant is added
- 🔄 **Continue Shopping** — Navigate back from cart to the product listing seamlessly

---

## Tech Stack

| Technology | Purpose |
|---|---|
| React 18 | UI components and rendering |
| Redux Toolkit | Global state management |
| React Redux | Connecting React components to the Redux store |
| Vite | Build tool and dev server |
| CSS | Component-level styling |

---

## Project Structure

```
e-plantShopping/
├── src/
│   ├── AboutUs.jsx          # About the company page
│   ├── App.jsx              # Root component and routing logic
│   ├── App.css              # Global styles and landing page background
│   ├── CartItem.jsx         # Shopping cart page component
│   ├── CartItem.css         # Cart styles
│   ├── CartSlice.jsx        # Redux slice — actions and reducer for cart state
│   ├── ProductList.jsx      # Product listing page component
│   ├── ProductList.css      # Product listing styles
│   ├── store.js             # Redux store configuration
│   └── main.jsx             # App entry point with Redux Provider
├── public/
├── package.json
└── README.md
```

---

## Redux State Management

The cart state is managed via a Redux slice (`CartSlice.jsx`) with three reducers:

- **`addItem`** — Adds a new plant to the cart, or increments quantity if it already exists
- **`removeItem`** — Removes a plant from the cart by name
- **`updateQuantity`** — Updates the quantity of a specific cart item

Action creators are exported as named exports and the reducer is the default export, consumed by `store.js`.

---

## Getting Started

### Prerequisites

- Node.js (v16 or above)
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/<your-username>/e-plantShopping.git

# Navigate into the project folder
cd e-plantShopping

# Install dependencies
npm install

# Run the app locally
npm run preview
```

The app runs on port **4173** by default.

---

## Deployment

This app is deployed using **GitHub Pages**.

```bash
# Install gh-pages
npm install gh-pages --save-dev

# Deploy
npm run deploy
```

Live URL: `https://<your-username>.github.io/e-plantShopping/`

---

## Plant Categories

The store features plants across five categories:

1. Air Purifying Plants
2. Aromatic Fragrant Plants
3. Insect Repellent Plants
4. Medicinal Plants
5. Low Maintenance Plants

---

