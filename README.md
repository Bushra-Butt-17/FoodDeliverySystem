

---

**🍔 FoodDeliverySystem**

A comprehensive web application that offers a seamless food ordering experience for customers and efficient order management for administrators. Users can easily browse menus, place orders, and track the status of their deliveries. Meanwhile, administrators have access to powerful tools for managing menu items, categories, and customer orders, ensuring smooth operations and an enhanced user experience.

---

## 📂 Project Structure  

```
FoodDeliverySystem/
├── assets/                     # Static resources (CSS, JavaScript, media)
├── partials-front/             # Reusable frontend components (headers, footers)
├── images/                     # Image files for the application
├── admin/                      # Backend admin panel files
├── config/                     # Configuration scripts
├── user/                       # Frontend files for user interactions
└── README.md                   # Documentation
```  

---

## ✨ Features  

### 🛍️ For Users:  
- **📖 Explore Menu:** Browse dishes by category or search for specific meals.  
- **🛒 Easy Ordering:** Add items to the cart and complete your purchase seamlessly.  
- **📦 Track Orders:** Stay updated on the real-time status of your orders.  
- **🌟 User-Friendly Interface:** Navigate through a sleek and responsive design.  

### 🛠️ For Admins:  
- **📑 Category Management:** Add, edit, and remove food categories with ease.  
- **🍽️ Menu Management:** Update menu items, their details, and pricing dynamically.  
- **📊 Order Management:** Monitor and update order statuses in real time.  
- **🔒 Secure Access:** Password-protected admin panel to ensure security.  

---

## 🛠️ Technologies Used  

### 🌐 **HTML (Hypertext Markup Language)**  
- **Purpose:** Provides the structure and content of web pages, including text, images, and forms.  
- **Role in This Project:**  
  - Defines the layout for user and admin interfaces.  
  - Organizes elements like navigation menus, forms, and data tables.  
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
- **Purpose:** Enhances the presentation and design of HTML elements, ensuring consistency and aesthetics.  
- **Role in This Project:**  
  - Creates responsive designs for desktops and mobile devices using media queries.  
  - Adds styling to buttons, navigation bars, and other UI components.  
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
- **Purpose:** Adds interactivity and dynamic behavior to web pages.  
- **Role in This Project:**  
  - Implements cart functionality, search functionality, and form validation.  
  - Updates the UI dynamically without refreshing the page using AJAX.  
- **Example:**  
  ```javascript  
  document.querySelector("#addToCart").addEventListener("click", function() {
      alert("Item added to cart!");
  });
  ```  

---

### ⚙️ **PHP (Hypertext Preprocessor)**  
- **Purpose:** A server-side scripting language for handling backend operations, database interactions, and dynamic content.  
- **Role in This Project:**  
  - Manages CRUD operations for orders, categories, and menu items.  
  - Handles admin authentication and session management.  
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
   Use tools like phpMyAdmin to import the `database.sql` file located in the `config` folder into your MySQL database.  

2. **Update Configuration**  
   Open `config/db-config.php` and update the file with your database credentials:  
   - **Host:** Your MySQL server (e.g., `localhost`)  
   - **Username:** Your database username  
   - **Password:** Your database password  
   - **Database Name:** The name of the imported database  

3. **Run the Application**  
   Place the project folder in your local server's root directory (e.g., `htdocs`) and access the system via your browser at:  
   `http://localhost/FoodDeliverySystem/`  

---

## 🎯 Future Enhancements  

- 🔐 **User Authentication:** Enable personalized user accounts for a tailored experience.  
- 💳 **Payment Gateway Integration:** Add secure online payment options.  
- 📝 **Ratings & Reviews:** Allow users to share feedback on dishes.  
- 📱 **Mobile Optimization:** Enhance the interface for a smoother mobile experience.  
- 🌍 **Multi-Language Support:** Cater to a wider audience with localization.  

---

