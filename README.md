# Delphi_Data_Table_Application
---

### **Purpose**
1. Collect user information such as:
   - Name
   - Roll Number
   - Age
   - Course
   - Marks
2. Display this data in a neat, table-like format on another window.
3. Allow users to delete all stored data if needed.

---

![img_20241128](https://github.com/user-attachments/assets/84967784-ed87-4880-8d8a-09ba567497b2)

### **How It Works**

#### **Form 1 (Main Form)**
- **Purpose**: Acts as the input form for entering data.
- **Features**:
  1. **Input Fields**: Contains text boxes for entering details (Name, Roll No, etc.).
  2. **Submit Button**:
     - When clicked, it saves the entered data into a list.
     - A message confirms that the data has been successfully stored.
  3. **Call Second Form Button**:
     - Opens a second form (window) where the stored data can be viewed.

---

#### **Form 2 (Second Form)**
- **Purpose**: Displays the collected data in a readable table format.
- **Features**:
  1. **Show Data Button**:
     - Displays the stored data in a memo box (a scrollable text area).
     - The data appears like a table with aligned columns (Name, Roll No, Age, etc.).
  2. **Delete Button**:
     - Clears all stored data.
     - Keeps the table header intact for future entries.

---

### **How It Behaves**
1. The user enters data in **Form 1** and clicks **Submit**.
   - Data gets saved in a list.
   - A success message confirms the action.

2. The user clicks **Call Second Form** to open **Form 2**.
   - In **Form 2**, clicking **Show Data** displays all the stored data in a structured format.

3. If the user clicks **Delete**, all data is cleared from the list.

---

![img_20241128(1)](https://github.com/user-attachments/assets/0e5f6a5a-c089-470e-bb2a-81075eb78ca0)

### **User Experience**
1. A smooth flow between two forms:
   - Form 1: Data Entry.
   - Form 2: Data Display and Management.
2. Simple and intuitive buttons for saving, viewing, and deleting data.

---

### **Key Technical Points**
- Data is stored in a **list** (`TStringList`), which acts like a temporary database.
- A **table-like format** is created using string formatting to align text neatly.
- The second form dynamically fetches data from the main form whenever required, ensuring both forms are synchronized.

---
![img_20241128(2)](https://github.com/user-attachments/assets/e3149209-5539-49c5-b9fc-ab5534aac11c)

