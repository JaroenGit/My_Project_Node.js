# Product Management System (Node.js + Express.js + EJS + MongoDB)
Introduction
---
```
This project is a basic full-stack product management system developed using Node.js and Express.js for the backend,
EJS (Embedded JavaScript) as the server-side template engine for frontend rendering, and MongoDB with Mongoose for database management.
The system also integrates Multer to handle product image uploads.
```
## 🧰 Installation and Configuration
package.json dependencies:
```json
"dependencies": {
  "ejs": "3.1.10",
  "express": "5.1.0",
  "mongoose": "8.15.2",
  "multer": "2.0.1",
  "nodemon": "^3.1.10"
}
```

## ⚙️Tools and Technologies

| Technology                | Functionality Description                                                    |
| ------------------------ | ------------------------------------------------------------ |
| **Node.js + Express.js** | Serves as the web server and handles routing requests and responses  |
| **MongoDB + Mongoose**   | Stores and manages product data using a NoSQL database structure                           |
| **EJS**                  | Renders HTML content dynamically on the server side     |
| **Multer**               | Manages image uploads and stores them in a designated directory                              |
| **Bootstrap / CSS**      | Provides responsive UI design and styling for the application interface                   |

## Database Setup
```
    - Import the productDB.product.json file into MongoDB.
    - If the database does not exist, MongoDB will automatically create it upon first access.
    - Verify that the connection URL is set to localhost:27017/productDB.
```

## 📁Project Structure
```
project_node_js/
├── models/               # Mongoose Schemas
│   └── product.js
├── routes/               # Routing files
│   └── myrouter.js
├── views/                # EJS templates
│   ├── index.ejs         # Product list view
│   ├── insert.ejs        # Product creation form
│   ├── show.ejs          # Product detail page
│   ├── header.ejs        # Reusable header template
│   ├── edit.ejs          # Product editing form
│   └── tabledata.ejs     # Product table layout
├── public/               # Static files (CSS, images)
│   ├── css/              # Stylesheets
│   └── img/products/     # Uploaded product images
├── app.js                # Application entry point
└── package.json
```

## System Features
```
  Product Listing — Displays all products with associated images.
  Add New Product — Users can input product details, upload an image, and store data in the database.
  Delete Product — Supports product deletion with confirmation prompts to prevent accidental removal.
  View Product Details — Retrieves detailed information using the product's _id from MongoDB.
  UI Styling — Uses Bootstrap and custom CSS files stored in /public for responsive and user-friendly design.
```
## System Usage
```
  - Home Page (/) Displays all products in the database along with their images.
  - Add Product (/insert) Form for entering name, price, size, description, and selecting an image file before clicking "Save."
  - View Product Details Click the "See More" button to view detailed product information.
  - Delete Product (/delete/:id) Sends a POST request to remove the selected product from the database after user confirmation.
```

# Run the server
```
# Run with Node.js
node app.js

# Run with Nodemon (auto-restart on file changes)
npx nodemon app.js

# Or configure a script in package.json
npm start
```

# ✍️ Developer Information
```
Full Name : Jaroen Sukcharoenchaiyakul
Gmail : jsaroen66@gmail.com
GitHub: github.com/JaroenGit
```
