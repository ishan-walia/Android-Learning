# 📌 Android Menus – Simple Definition Notes

## ✅ What is a Menu in Android?
Menu is a part of Android UI that provides users with options and actions.  
It helps users navigate easily inside the app.

Android recommends creating menus using **XML**, because it keeps the code clean, organized, and easy to maintain.

---

## ✅ How Menus Are Defined?
- Menus are created inside the **res/menu/** folder  
- Each menu has its own **XML file**  
- Menu items are written using `<item>` tags  

---

## ✅ Example of Simple Menu (Mail, Upload, Share)
This type of menu contains three normal items:
- Mail  
- Upload  
- Share  

---

## ✅ Different Tags in Menu XML

### **1️⃣ `<menu>`**
- Root element  
- Holds all menu items  

### **2️⃣ `<item>`**
- Defines a single menu item  
- Contains: **title**, **icon**, **id**  
- Can have a nested `<menu>` to create a **submenu**  

### **3️⃣ `<group>`**
- Optional  
- Used to group multiple items  
- Helps manage: visibility, enable/disable, checkable behavior  

---

## ✅ Sub Menu (File → Create New, Open)
Submenu means:
- **One main item** → Inside it, **more child items**

Example:
- File  
  - Create New  
  - Open  

Useful when one main option contains related actions.

---

## ✅ Types of Menus in Android

### **1️⃣ Options Menu**
- Main menu shown in the AppBar (3-dot menu)  
- Used for global actions like **Search**, **Settings**, etc.  

### **2️⃣ Context Menu**
- Opens on **long-press**  
- Shows actions related to the selected item (Edit, Delete)  

### **3️⃣ Popup Menu**
- Small vertical menu  
- Opens next to the view that triggers it  
- Used for overflow actions  

---

### menu_example.xml:
```xml

<?xml version="1.0" encoding="utf-8"?>
<menu 
    xmlns:android="http://schemas.android.com/apk/res/android">
    <item 
        android:id="@+id/mail"
        android:icon="@drawable/mail"
        android:title="Mail" 
        />
    
    <item 
        android:id="@+id/upload"
        android:icon="@drawable/upload"
        android:title="Upload"
        />
    
    <item 
        android:id="@+id/share"
        android:icon="@drawable/share"
        android:title="Share" 
        />
</menu>

```


### menu_example.xml:
```

<?xml version="1.0" encoding="utf-8"?>
<menu 
    xmlns:android="http://schemas.android.com/apk/res/android">
    <item 
        android:id="@+id/file"
        android:title="File" >
        
        <!-- "File" submenu -->
        <menu>
            <item 
                android:id="@+id/create_new"
                android:title="Create New" 
                />
            <item 
                android:id="@+id/open"
                android:title="Open" 
                />
        </menu>
    </item>
</menu>

```

