# 📌 CardView in Android – Complete Notes (Simple & Clean)

## ✅ What is CardView?
CardView is a UI component in Android used to display content inside a rectangle with **rounded corners** and **shadow (elevation)**.  
It gives a modern and clean material-design look to the UI.

### ⭐ Features
- Looks like physical cards  
- Supports elevation (shadow)  
- Works on all Android versions  
- Commonly used inside RecyclerView  

---

## 📍 Where is CardView Used?
- List items (shopping apps, news apps)  
- Dashboards  
- Profile cards  
- RecyclerView items  

---

## 📝 Important XML Attributes of CardView

| Attribute | Meaning |
|----------|---------|
| `app:cardCornerRadius` | Sets rounded corners |
| `app:cardBackgroundColor` | Sets background color |
| `app:cardElevation` | Adds shadow (depth) |
| `app:cardMaxElevation` | Sets maximum shadow level |
| `app:useCompatPadding` | Prevents shadow from getting clipped |

---

# ⚙️ How to Implement CardView

## 🧩 Step 1: Create New Android Project
- Choose **Java/Kotlin**  
- Select **Empty Activity**

---

## 🧩 Step 2: Add CardView Dependency  
Add this line inside your `build.gradle (Module:)`:
```gradle
implementation "androidx.cardview:cardview:1.0.0"
```

🧩 Step 3: Add Google Repository

Inside settings.gradle.kts:
```kotlin
buildscript {
    repositories {
        google()
        mavenCentral()
    }
}
```

🧩 Step 4: Create CardView in activity_main.xml

```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/white">

    <androidx.cardview.widget.CardView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_margin="24dp"
        app:cardElevation="24dp"
        app:cardCornerRadius="24dp"
        app:layout_constraintTop_toTopOf="parent">

        <androidx.constraintlayout.widget.ConstraintLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">

            <ImageView
                android:id="@+id/imageView2"
                android:layout_width="100dp"
                android:layout_height="100dp"
                android:layout_margin="24dp"
                android:src="@drawable/gfg_logo"
                app:layout_constraintStart_toStartOf="parent"
                app:layout_constraintTop_toTopOf="parent" />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="GeeksforGeeks"
                android:textSize="24sp"
                android:textColor="@color/black"
                android:textStyle="bold"
                app:layout_constraintStart_toEndOf="@+id/imageView2"
                app:layout_constraintTop_toTopOf="parent"
                app:layout_constraintBottom_toBottomOf="parent"/>

        </androidx.constraintlayout.widget.ConstraintLayout>

    </androidx.cardview.widget.CardView>

</androidx.constraintlayout.widget.ConstraintLayout>

```



## 📱 Output
Your app will display:
<li>Image on the left</li>
<li>Text on the right</li>
<li>Rounded corners</li>
<li>Shadow (elevation)</li>'

# 🖼 Screenshot

(Add your screenshot here)

<img src="your_screenshot_link_here" width="300">

