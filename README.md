# 🍽️ Restaurant Management System (Oracle SQL)

This is a collaborative **Oracle SQL-based Restaurant Management System** designed to model a real-world restaurant ecosystem. The project includes all major components like customers, waiters, inventory, menu, orders, reviews, and recommendations.

---

## ✨ Features

- **Cuisine & Restaurant Management**: Add and fetch restaurant data by cuisine type.
- **Waiter Operations**: Hire waiters, view all waiters in a restaurant, and calculate total tips by waiter and state.
- **Menu & Inventory**: Add menu items, manage restaurant inventory, and generate inventory reports.
- **Customer & Orders**: Add customers, place orders, and automatically update inventory.
- **Review & Recommendations**: Add and analyze reviews, and generate restaurant recommendations.

---

## 🗂️ Schema Overview

### Tables
- `Cuisine_Types`
- `Restaurants`
- `Waiters`
- `Menu_Items`
- `Restaurant_Inventory`
- `Customers`
- `Orders`
- `Reviews`
- `Recommendations`

### Sequences
Used for auto-incrementing primary keys in all major tables (e.g., `Restaurant_ID_Seq`, `Customer_ID_SEQ`, etc.)

### Functions
Helper functions for:
- `FIND_CUISINE_TYPE_ID`
- `FIND_RESTAURANT_ID`
- `FIND_WAITER_ID`
- `FIND_MENU_ITEM_ID`
- `FIND_CUSTOMER_ID`

---

## ⚙️ Core Procedures

### Member 1 - Cuisine & Restaurants
- `ADD_Cuisine_Type`
- `ADD_Restaurant`
- `Restaurant_By_Cuisine_Type`
- `Report_Income_By_State`

### Member 2 - Waiters
- `ADD_WAITER`
- `LIST_WAITERS`
- `CalculateTotalTipOfWaiter`
- `CalculateTipsbyState`

### Member 3 - Menu & Inventory
- `CREATE_MENU_ITEM`
- `ADD_ITEM_INVENTORY`
- `Generate_Menu_Item_Report`
- `UPDATE_MENU_ITEM_INVENTORY`

### Member 4 - Customers & Orders
- `Add_Customer`
- `Place_Order`

### Member 5 - Reviews & Recommendations
- `Add_Review`
- `BUY_OR_BEWARE`
- `RECOMMEND_TO_CUSTOMER`
- `List_Recommendations`

---

## 🔁 Trigger

- `UPDATE_INVENTORY_AFTER_ORDER`: Automatically reduces inventory quantity after each new order.

---

## 🛠️ How to Run

1. Use any Oracle-compatible environment (e.g., SQL Developer, Oracle Live SQL).
2. Load and execute the full script sequentially.
3. Make sure to enable output:
   ```sql
   SET SERVEROUTPUT ON;
4. Run anonymous blocks to populate initial data and test procedures

---

## Notes:
- This system simulates a restaurant's backend and can be extended further with UI integrations or API hooks.
- Contributions from each team member are modular and well-commented for readability.

---

## License:
- This project is developed for academic and educational purposes. Feel free to fork, clone, and enhance it for learning.

---

## Acknowledgements:
- Thanks to our instructors, classmates, and contributors who helped shape this collaborative database system.
