🐄 Bufflos Business Manager

A Flutter-based offline business management app for managing two separate business modules — Milk Business and Food Business — with full CRUD operations, real-time reporting, and chart analytics. Built for Android with a clean Material Design UI.




✨ Features

🥛 Milk Business Module


Manage Milk Sellers and Milk Customers
Record daily Milk Purchases and Sales
Auto-calculate profit per transaction
Today / Week / Month / All-Time Reports
Bar chart for 7-day sales trend
Top customers & sellers ranking


🛒 Food Business Module


Manage Food Products with stock tracking
Manage Food Suppliers and Customers
Record Purchases and Sales
Automatic stock deduction on sale
Full Sales & Purchase Reports
Bar chart for 7-day food sales


⚙️ Core Features


📦 Offline-first — SQLite local database (no internet required)
🔍 Search & Filter on all records
✏️ Full CRUD — Add, Edit, Delete on every screen
📊 Dashboard with today's summary cards
🎨 Clean Material 3 light theme
📱 Supports Android 5.0+ (API 21+)
🔒 Data isolation — Milk and Food data never mix



🗂️ Project Structure

bufflos_business/
├── lib/
│   ├── main.dart                  # App entry point
│   ├── theme/
│   │   └── app_theme.dart         # Colors & Material theme
│   ├── db/
│   │   └── db_helper.dart         # SQLite database & all CRUD
│   ├── models/
│   │   ├── milk_seller.dart
│   │   ├── milk_customer.dart
│   │   ├── milk_purchase.dart
│   │   ├── milk_sale.dart
│   │   ├── food_product.dart
│   │   ├── food_supplier.dart
│   │   ├── food_customer.dart
│   │   ├── food_purchase.dart
│   │   └── food_sale.dart
│   ├── widgets/
│   │   └── widgets.dart           # Shared reusable UI components
│   └── screens/
│       ├── home_screen.dart       # Home dashboard + bottom nav
│       ├── milk/                  # Milk module (6 screens)
│       │   ├── milk_module.dart
│       │   ├── milk_dashboard.dart
│       │   ├── milk_sellers.dart
│       │   ├── milk_customers.dart
│       │   ├── milk_purchases.dart
│       │   ├── milk_sales.dart
│       │   └── milk_reports.dart
│       └── food/                  # Food module (7 screens)
│           ├── food_module.dart
│           ├── food_dashboard.dart
│           ├── food_products.dart
│           ├── food_suppliers.dart
│           ├── food_customers.dart
│           ├── food_purchases.dart
│           ├── food_sales.dart
│           └── food_reports.dart
├── android/                       # Android native config
├── pubspec.yaml
└── README.md


🗄️ Database Schema

SQLite database with 9 tables:

TablePurposemilk_sellersMilk supplier recordsmilk_customersMilk buyer recordsmilk_purchasesDaily milk purchase entriesmilk_salesDaily milk sale entriesfood_productsProduct catalog with stockfood_suppliersFood supplier recordsfood_customersFood buyer recordsfood_purchasesFood purchase entriesfood_salesFood sale entries


🛠️ Tech Stack

TechnologyUsageFlutter 3.xUI frameworkDart 3.xProgramming languagesqfliteSQLite local databasefl_chartBar chart visualizationsintlDate & number formatting


🚀 Getting Started

Prerequisites


Flutter SDK 3.10+
Android Studio with Android SDK
Java 17+


Run Locally

bash# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/bufflos-business.git
cd bufflos-business

# 2. Install dependencies
flutter pub get

# 3. Run on connected device or emulator
flutter run

Build APK

bash# Standard release APK
flutter build apk --release

# Split APKs (smaller file sizes, recommended)
flutter build apk --split-per-abi --release

APK output location:

build/app/outputs/flutter-apk/app-release.apk


📦 Dependencies

yamldependencies:
  sqflite: ^2.3.3     # SQLite database
  path: ^1.9.0        # File path utilities
  intl: ^0.19.0       # Internationalization & formatting
  fl_chart: ^0.68.0   # Beautiful charts





👨‍💻 Author

Asadullah

Flutter Developer | CS Student

📍 Pakistan



