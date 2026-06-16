# Pharmacy Management System

A comprehensive GUI-based pharmacy management application built with Java Swing. This system provides an intuitive interface for managing pharmacy operations including inventory, sales, billing, customer management, and reporting.

## 📋 Features

### ✅ User Authentication & Access Control
- Secure login with username and password
- Role-based access control:
  - **Admin**: Full access to all features
  - **Staff**: Limited access (Sales and Customer management only)
- Account locking after 3 consecutive failed attempts (5 minutes)
- SHA-256 password hashing
- Session management

### ✅ Inventory Management (Admin Only)
- Add, edit, and delete medicines
- Track stock quantities and reorder levels
- Monitor expiry dates with alerts (30-day warning)
- Low-stock alerts
- Search and filter medicines by name, category, or batch number

### ✅ Sales & Billing
- Create new sales transactions
- Search and add medicines to cart
- Calculate totals with discount support
- Generate printable bills
- Automatic inventory deduction after sale

### ✅ Customer Management
- Add and manage customer records
- Track purchase history
- Search customers by name/phone
- View customer spending patterns

### ✅ Supplier Management (Admin Only)
- Add, edit, and delete supplier records
- Store supplier contact information
- Associate suppliers with medicines
- Track supplier details

### ✅ Reports
- Sales reports
- Inventory reports
- Expiry reports
- Low stock reports
- Export functionality

### ✅ Dashboard
- Real-time statistics
- Total medicines count
- Low stock items alert
- Medicines expiring soon
- Today's sales summary

## 🛠️ Technology Stack

| Component | Technology |
|-----------|------------|
| Language | Java 11+ |
| GUI Framework | Java Swing |
| Build Tool | Maven |
| Version Control | Git & GitHub |
| IDE | VS Code / NetBeans |

## 📁 Project Structure

```
pharmacy-management-system/
├── src/main/java/com/pharmacy/
│   ├── PharmacyApp.java                (Entry point)
│   ├── ui/
│   │   ├── LoginFrame.java             (Login screen)
│   │   ├── MainFrame.java              (Main window with sidebar)
│   │   ├── DashboardPanel.java         (Dashboard)
│   │   ├── InventoryPanel.java         (Inventory management)
│   │   ├── SalesPanel.java             (Sales & billing)
│   │   ├── CustomerPanel.java          (Customer records)
│   │   ├── SupplierPanel.java          (Supplier management)
│   │   ├── ReportsPanel.java           (Reports)
│   │   └── SettingsPanel.java          (Admin settings)
│   ├── models/
│   │   ├── User.java
│   │   ├── Medicine.java
│   │   ├── Customer.java
│   │   ├── Supplier.java
│   │   ├── Bill.java
│   │   └── BillItem.java
│   └── utils/
│       ├── Constants.java
│       ├── ValidationUtils.java
│       ├── UIUtils.java
│       └── SessionManager.java
├── pom.xml
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Java 11+ installed
- Maven 3.6+ installed
- Git installed
- VS Code with Extension Pack for Java (optional)

### Installation & Running

#### Option 1: Using Maven (Command Line)
```bash
git clone https://github.com/rabiya-zainab/pharmacy-management-system.git
cd pharmacy-management-system
mvn clean install
mvn exec:java -Dexec.mainClass="com.pharmacy.PharmacyApp"
```

#### Option 2: Using VS Code
1. Clone and open the project in VS Code
2. Install "Extension Pack for Java"
3. Run commands from Option 1

#### Option 3: Create Executable JAR
```bash
mvn clean package
java -jar target/pharmacy-management-system-1.0.0.jar
```

## 👤 Test Credentials

| Role | Username | Password |
|------|----------|----------|
| Admin | admin | admin123 |
| Staff | staff | staff123 |

## 🎨 UI/UX Design
- Color Scheme: Blue & White professional theme
- Responsive Layout
- Sidebar navigation
- Real-time form validation
- Professional fonts
- Accessible components

## ⚠️ Important Notes

Currently frontend-only. To integrate with a database:
- Set up SQLite/MySQL/PostgreSQL
- Create schema based on models
- Implement DAO/Repository layer
- Connect UI with DB

## 🔐 Security Features
- SHA-256 password hashing
- Account locking
- Session-based authentication
- Role-based access control
- Input validation

## 🔄 Future Enhancements
- Database integration
- Backend API integration
- Advanced reporting with charts
- Prescription management
- Multi-user logging
- Email notifications
- Barcode scanning
- Mobile app version

## 📝 License
Open source under MIT License.

## 👨‍💻 Author
Rabiya Zainab - @rabiya-zainab

## 📞 Support
For issues, feature requests, or questions, contact Rabiya Zainab.
