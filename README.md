# 🏪 Inventory Management System (Structured Programming)

This project is a Structured (Non-OOP) Inventory Management System developed in C++, designed to demonstrate core programming concepts such as data structures, file handling, searching, sorting, and user-driven menu operations. The system allows efficient handling of essential inventory tasks

---

## 🧩 Features Overview

| Feature | Description |
|----------|--------------|
| ➕ **Add Item** | Insert new product with ID, name, price, and quantity |
| 👀 **View All Items** | Display all items grouped by category |
| 🔄 **Update Quantity** | Modify the stock of existing items |
| ❌ **Delete Item** | Remove item by ID |
| ⚠️ **Low Stock Report** | Show all items with quantity ≤ 5 |
| 💾 **Save & Load** | Save and load data using a binary file (`inventory.dat`) |
| 🗂️ **Category Management** | Manage categories like *Electronics*, *Books*, etc. |
| 🧠 **Dynamic Memory** | Implemented using `new` and `delete[]` |
| 🔍 **Pointers** | Used in searching and item management |

---

## 🧾 Main Menu (Program Display)




## ⚙️ Explanation of Each Option



### ===== INVENTORY MANAGEMENT SYSTEM =====

- **Add Category**

- **Add Item**

- **View All Items**

- **Update Quantity**

- **Delete Item**

- **Low Stock Report**

- **Save Data**

- **Exit**



### 🟩 **1️⃣ Add Category**

**Description:**  
Adds a new category like *Electronics*, *Books*, etc.  
The program stores it dynamically.

**Sample Output:**

```
Enter new category name: Electronics
Category 'Electronics' added successfully!

Enter new category name: Books
Category 'Books' added successfully!
```


✅ *Now you have 2 categories stored in memory.*

---

### 🟦 **2️⃣ Add Item**

**Description:**  
Lets you add a new item in a specific category.  
Input includes Category Name → ID → Item Name → Price → Quantity.

**Sample Output:**

```
Enter your Choice (1-8): 2

---- Available Categories ----
1. Electronics
2. Cosmetics

Select category number to add item: 1

Enter Item ID: 101
Enter Item Name: Laptop
Enter Price: 85000
Enter Quantity: 8
Item added successfully to category 'Electronics'!
```


✅ *This item is now stored under the Electronics category.*

---

### 🟨 **3️⃣ View All Items**

**Description:**  
Displays all items grouped by category.  
If no items are available, a message appears.

**Sample Output:**

```
===== INVENTORY LIST =====

Category: Electronics

ID Name Price Qty
101 Laptop 85000 8
102 Headphones 3500 12

Category: Books

ID Name Price Qty
201 C++ Primer 1500 3
```


✅ *All stored data displayed clearly.*

---

### 🟧 **4️⃣ Update Quantity**

**Description:**  
Used to modify stock quantity of any existing item using its ID.

**Sample Output:**

```
Enter Item ID to update: 101
Current Quantity: 8
Enter New Quantity: 12
Quantity updated successfully!
```


✅ *Item 101 (Laptop) now has quantity 12.*

---

### 🟥 **5️⃣ Delete Item**

**Description:**  
Removes an item from the inventory using its ID.  
It searches all categories and deletes the item if found.

**Sample Output:**

```
Enter Item ID to delete: 201
Item found in category 'Books'
Item deleted successfully!
```


✅ *Now “C++ Primer” is removed from the Books category.*

---

### 🟪 **6️⃣ Low Stock Report**

**Description:**  
Lists all items whose quantity ≤ 5.  
This helps you identify which products need restocking.

**Sample Output:**

```
===== LOW STOCK ITEMS (Qty ≤ 5) =====

Category: Books

ID Name Price Qty
301 Python Guide 1200 2

Category: Electronics

ID Name Price Qty
104 Mouse 800 4
```


✅ *These items are running low and should be restocked.*

---

### 🟫 **7️⃣ Save Data**

**Description:**  
Saves all inventory data (categories + items) into a binary file named `inventory.dat`.

**Sample Output:**

```
Saving data...
Data saved successfully in inventory.dat
```


✅ *Your data is safely saved on disk.*

---

### ⚫ **0️⃣ Exit**

**Description:**  
Before exiting, the program saves all data automatically and frees memory.

**Sample Output:**

```
Saving data...
Data saved successfully!
Exiting program... Goodbye!
```


✅ *Program ends safely and all memory is freed.*



---

## 💾 File Handling

- All data is saved in **binary format** (`inventory.dat`)
- When program starts → data is automatically **loaded**
- When program exits → data is automatically **saved**

---
