# MI Lifestyle Products – Official Price List

This is a simple, mobile-friendly HTML webpage that displays product price lists for **MI Lifestyle** products, categorized by type, with separate pricing for **sellers (wholesale/distributors)** and **customers (retail)**. The page is built for Tamil-speaking users and integrates WhatsApp for easy ordering.

## 🔗 Live Page

You can view the hosted page here:  
👉 [https://neyakkoot.github.io/MiLifeStyle_Products_Details_Prize/](https://neyakkoot.github.io/MiLifeStyle_Products_Details_Prize/)

> **Note**: The page requires an accompanying `style.css` and `list.js` file (or similar assets) to fully function.

## 📂 Project Structure
project-root/
│
├── index.html # Main HTML file
├── style.css # Styles (referenced in HTML)
├── list.js # Product data (referenced in HTML)
└── README.md # Project documentation

text

## ✨ Features

- **Category-based product listing**  
  - Health Care  
  - Personal Care  
  - Food & Beverage  
  - Home Care  
  - Agro Care  
  - Certificate Course on Direct Selling  

- **Dual pricing model**  
  - **Seller price** (for distributors/wholesale)  
  - **Customer price** (retail)

- **WhatsApp integration**  
  - Customers can directly message a seller to place an order.  
  - Sellers can contact a dedicated number for bulk purchases.

- **Image viewer**  
  - Click on **"View Image"** to see product photos with zoom support.

- **Responsive layout**  
  - Works on desktops, tablets, and mobile devices.

## 🛠️ How It Works

1. **Category Cards** – Click on any category card to display its products.
2. **Product Grid** – Each product shows two action buttons:  
   - 📷 **View Image** – Opens a modal with product photo.  
   - 💰 **Seller Price** – Shows seller contact info and a WhatsApp link.  
   - 🛒 **Customer Price** – Direct WhatsApp link to place an order.
3. **Popups (Modals)** – Used for seller info and image zoom.
4. **Footer** – Displays a main WhatsApp contact number.

## 📝 Dependencies

- **CSS**: `style.css` (assumed to provide styling for cards, grids, buttons, modals)
- **JavaScript**: `list.js` (must define `products` array and `imgBase` variable)

### Expected `list.js` format example:

```javascript
const imgBase = "images/"; // base path for product images

const products = [
  {
    cat: "HC",
    name: "Sample Health Product",
    r: 250.00,   // seller price
    m: 299.00,   // customer price
    img: "sample.jpg"
  },
  // more products...
];
cat should be one of: "HC", "PC", "FB", "HM", "AG"

r = seller price, m = customer price

📱 WhatsApp Numbers Used
Customer orders: +91 63694 13436 (as per footer)

Seller inquiries: 9600370671 (hardcoded in openSellerPopup)

⚠️ Notes
The page currently has duplicate id="HC" for two different sections. This may cause display issues. It's recommended to fix the duplicate IDs in the HTML.

All product data must be maintained inside list.js.

Image zoom functionality is CSS-based (transform:scale) and not a true zoom library.

🚀 Future Improvements
Fix duplicate id="HC" in HTML.

Add search/filter functionality.

Use dynamic product loading from a JSON API.

Add admin panel to update prices and products.

🧾 License
This project is for informational and business use. You may modify and use it as needed for your MI Lifestyle product distribution.

Maintained by: MI Lifestyle Distributor Team
Last Price Update: 16.11.2024

text

---

Let me know if you’d like a shorter version, a developer setup guide, or help generating the required `style.css` and `list.js` template files.
