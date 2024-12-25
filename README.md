
---

# **🍔 FoodDeliverySystem**

A robust and scalable web application designed to deliver an intuitive food ordering experience for customers while providing administrators with powerful tools for order and menu management. The platform allows users to explore menus, place orders, track delivery statuses, and enjoy a seamless ordering experience. Meanwhile, administrators benefit from easy-to-use features for managing food categories, menu items, and orders, ensuring smooth operational workflows and an optimized user experience.

---

## 📂 Project Structure

```
FoodDeliverySystem/
├── assets/                     # Static resources (CSS, JavaScript, media files)
├── partials-front/             # Reusable frontend components (headers, footers, modals)
├── images/                     # Image files for the application
├── admin/                      # Backend admin panel files and scripts
├── config/                     # Configuration scripts for database and environment settings
├── user/                       # Frontend files for user interactions (UI components, user-specific logic)
├── README.md                   # Project documentation
```

---

## ✨ Features

### 🛍️ For Users:
- **📖 Explore Menu:** Browse dishes by category, cuisine, or search for specific meals.
- **🛒 Easy Ordering:** Select items, add them to the cart, and complete the purchase process seamlessly with real-time updates.
- **📦 Track Orders:** Stay informed about the real-time status of orders, from preparation to delivery.
- **🌟 User-Friendly Interface:** A responsive and visually appealing design ensures a smooth experience across desktop and mobile platforms.
- **🔄 Realtime Updates:** Experience live order status updates via AJAX, with no need to refresh the page.
  
### 🛠️ For Admins:
- **📑 Category Management:** Add, update, or remove food categories to ensure easy menu navigation for customers.
- **🍽️ Menu Management:** Efficiently update menu items, their descriptions, prices, and availability.
- **📊 Order Management:** Monitor and manage incoming orders, update their statuses (e.g., Pending, In Progress, Delivered), and track historical data.
- **🔒 Secure Admin Panel:** Admin access is protected by a robust authentication system, ensuring security and control.
- **📈 Reporting:** Access real-time insights and reports on sales, most popular dishes, and order trends.
  
---

## 🛠️ Technologies Used

### 🌐 **HTML (Hypertext Markup Language)**
- **Purpose:** Provides the structure and layout of the web pages, including content organization such as text, images, and forms.
- **Role in This Project:**  
  - Defines the overall page structure for both user and admin interfaces.
  - Organizes elements like menus, forms, and order data in a meaningful, user-friendly manner.
- **Example:**  
  ```html
  <div class="menu-item">
      <h3>Cheese Burger</h3>
      <p>$10</p>
      <button>Add to Cart</button>
  </div>
  ```

---

### 🎨 **CSS (Cascading Style Sheets)**
- **Purpose:** Responsible for the visual appearance and layout of the web pages, ensuring that the content is presented in a clean, professional, and aesthetically pleasing manner.
- **Role in This Project:**  
  - Implements responsive design techniques using media queries for mobile and desktop versions.
  - Enhances user experience with styling for buttons, navigation bars, cards, and other UI components.
- **Example:**  
  ```css
  .menu-item {
      background-color: #f9f9f9;
      padding: 20px;
      border-radius: 8px;
      text-align: center;
  }
  button {
      background-color: #ff5722;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
  }
  ```

---

### 🤖 **JavaScript**
- **Purpose:** Adds dynamic behavior and interactivity to the website, allowing for real-time updates without needing to refresh the page.
- **Role in This Project:**  
  - Implements core functionality like cart operations, real-time order tracking, and search features.
  - Utilizes AJAX to fetch data dynamically and update the UI without page reloads.
  - Validates forms, ensuring users enter correct data.
- **Example:**  
  ```javascript
  document.querySelector("#addToCart").addEventListener("click", function() {
      alert("Item added to cart!");
  });
  ```

---

### ⚙️ **PHP (Hypertext Preprocessor)**
- **Purpose:** Server-side scripting language that handles backend logic, data processing, and interactions with the database.
- **Role in This Project:**  
  - Manages CRUD (Create, Read, Update, Delete) operations for food items, categories, and orders.
  - Handles user authentication for the admin panel and maintains session management.
  - Ensures smooth communication between the front end and the MySQL database.
- **Example:**  
  ```php
  // Fetch menu items from the database
  $query = "SELECT * FROM menu_items";
  $result = $conn->query($query);
  while ($row = $result->fetch_assoc()) {
      echo "<div class='menu-item'>";
      echo "<h3>{$row['name']}</h3>";
      echo "<p>\${$row['price']}</p>";
      echo "</div>";
  }
  ```

---

## 🚀 Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Bushra-Butt-17/FoodDeliverySystem.git
cd FoodDeliverySystem
```

### 2️⃣ Set Up the Database
1. **Import the Database Schema**  
   Import the `database.sql` file from the `config` folder into your MySQL database using phpMyAdmin or a similar database management tool.

2. **Update Database Configuration**  
   Edit the `config/db-config.php` file and provide your database credentials:
   - **Host:** The host address of your MySQL server (e.g., `localhost`).
   - **Username:** Your MySQL username.
   - **Password:** Your MySQL password.
   - **Database Name:** The name of the database you imported from `database.sql`.

3. **Run the Application**  
   Place the project folder into your local server's root directory (e.g., `htdocs`) and access it through your browser at:
   `http://localhost/FoodDeliverySystem/`

---

## 🎯 Future Enhancements

- 🔐 **User Authentication:** Integrate a secure login system for users to manage their personal information, order history, and preferences.
- 💳 **Payment Gateway Integration:** Implement payment functionality for users to complete purchases securely via integrated payment processors (e.g., Stripe, PayPal).
- 📝 **Ratings & Reviews:** Allow customers to rate and leave reviews for dishes, enhancing the decision-making process for other users.
- 📱 **Mobile Optimization:** Further optimize the UI for mobile devices, ensuring a smooth and intuitive experience for users on-the-go.
- 🌍 **Multi-Language Support:** Expand accessibility by offering localization options to support multiple languages and cater to a wider audience.

---

