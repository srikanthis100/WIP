# Meal Planner & Pantry Tracker

A lightweight, single-file web application built with vanilla HTML, CSS, and JavaScript. It helps users manage daily meal plans, track pantry inventory, customize themes based on meal times, and import/export data via CSV.

---

## 🌟 Key Features

* **Meal Planner & Dashboard:** Displays the active meal slot (Breakfast, Lunch, or Dinner) alongside upcoming meals, dietary badges, prep notes, and interactive options to mark meals as cooked or shuffle options.
* **Pantry Management:** Track stock levels with automated percentage indicators and status badges (Full, Low, Out). Includes flexible sorting options (Urgency/Stock Level, Category, Name) and soft-deletion with restoration capabilities.
* **Time-Aware Auto Themes:** Dynamically switches theme styles (Sunrise Citrus, Midday Forest, Midnight Obsidian) based on the time of day, with optional manual overrides and a built-in theme editor.
* **Accordion-Style Settings:** Compact, expandable settings interface for configuring themes, importing/exporting CSVs, and wiping application data.
* **CSV Data Import/Export:** Robust, quote-aware CSV parser to import and export both pantry inventories and meal lists.
* **Local Persistence:** Retains all user data, custom themes, and meal history in browser `localStorage`.

---

## 🛠️ Project Structure

The application is fully contained within a single `index.html` file, requiring no build steps, bundlers, or external framework dependencies.

```text
├── index.html          # Single-file HTML/CSS/JS application
└── README.md           # Project documentation
```

## 🚀 Getting Started
1. Download or clone the repository containing `index.html`.
2. Double-click `index.html` or open it directly in any modern web browser (Chrome, Firefox, Safari, Edge).
3. The app will initialize with default test data automatically.

## 📖 CSV Data Formats
### Pantry CSV Export/Import Format
```
Category,Item,Required-Stock,Available-Stock
"Foodgrains, Oil & Masala","Rice",1000,500
"General","Salt",2,1
```

### Meals CSV Export/Import Format
```
Name,Category,DietType,Tags,PrepNote
"Oatmeal & Berries","Breakfast","veg","Quick;Healthy",""
"Paneer Masala & Roti","Dinner","veg","Festive","Soak paneer"
```

## 🎨 Auto-Theme Schedule
* Breakfast Slot: 6:00 AM – 11:00 AM
* Lunch Slot: 11:00 AM – 4:00 PM
* Dinner Slot: 4:00 PM – 6:00 AM

## 🔮 Future Enhancements
Firebase Authentication and Cloud Firestore integration for multi-device real-time sync.