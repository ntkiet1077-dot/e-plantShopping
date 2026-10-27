# Paradise Nursery Shopping Application

Paradise Nursery is an online plant shopping application where plant enthusiasts can explore, discover, and purchase a curated collection of houseplants. Built with React and Redux Toolkit, the application delivers a seamless, responsive, and intuitive e-commerce experience.

## Project Overview

- **Project Name:** Paradise Nursery Shopping Application
- **Course:** Developing Front-End Apps with React (IBM Skills Network / Coursera)
- **Built with:** React, Redux Toolkit, Vite, CSS3, HTML5

## Key Features

1. **Landing Page:**
   - Welcome banner featuring the brand slogan: *"Where Green Meets Serenity"*.
   - Immersive background visual and an "About Us" section highlighting Paradise Nursery's mission and commitment to greener spaces.
   - A prominent "Get Started" call-to-action button that smoothly navigates to the plant catalog.

2. **Houseplant Catalog & Categories:**
   - 30 unique houseplants organized into 5 distinct categories:
     - *Air Purifying Plants* (Snake Plant, Spider Plant, Peace Lily, Boston Fern, Rubber Plant, Aloe Vera)
     - *Aromatic Fragrant Plants* (Lavender, Jasmine, Rosemary, Mint, Lemon Balm, Hyacinth)
     - *Insect Repellent Plants* (Oregano, Marigold, Geraniums, Basil, Lavender, Catnip)
     - *Medicinal Plants* (Aloe Vera, Echinacea, Peppermint, Lemon Balm, Chamomile, Calendula)
     - *Low Maintenance Plants* (ZZ Plant, Pothos, Snake Plant, Cast Iron Plant, Succulents, Aglaonema)
   - Each plant card displays a high-resolution thumbnail, name, description, and price.

3. **Interactive Shopping Cart:**
   - "Add to Cart" button on each card that dispatches actions to Redux Toolkit.
   - Button turns to "Added to Cart" and is disabled once the item is in the cart to prevent duplicate single additions.
   - Persistent top navigation bar visible across both catalog and cart views with direct navigation links:
     - Home
     - Plants
     - Shopping Cart icon with dynamic badge count showing total quantity of items.
   - Cart View displaying:
     - Total cart amount calculated dynamically.
     - Itemized list with thumbnail, plant name, unit price, and subtotal.
     - Increment (`+`) and decrement (`-`) quantity controls with automatic recalculation.
     - Delete button to remove items.
     - "Continue Shopping" button returning to the product catalog.
     - "Checkout" button displaying a coming soon prompt.

## Project Structure

```text
e-plantShopping/
├── public/
├── src/
│   ├── assets/
│   ├── AboutUs.css
│   ├── AboutUs.jsx       # About Us component with company details
│   ├── App.css           # Landing page and global styling
│   ├── App.jsx           # Main App component with landing page & navigation
│   ├── CartItem.css      # Cart page styling
│   ├── CartItem.jsx      # Shopping cart component with quantity controls & totals
│   ├── CartSlice.jsx     # Redux slice managing cart state (addItem, removeItem, updateQuantity)
│   ├── index.css
│   ├── main.jsx          # Root entry point with Redux Provider
│   ├── ProductList.css   # Product grid and navigation styling
│   ├── ProductList.jsx   # Product catalog component grouped by categories
│   └── store.js          # Redux store configuration
├── index.html
├── package.json
└── README.md
```

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/e-plantShopping.git
   cd e-plantShopping
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
4. Build for production:
   ```bash
   npm run build
   ```

## License
This project is licensed under the MIT License.
