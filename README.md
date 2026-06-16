Pharmacy Management System
A comprehensive GUI-based pharmacy management application built with Java Swing. This system provides an intuitive interface for managing pharmacy operations including inventory, sales, billing, customer records, and supplier management.

📋 Features
✅ User Authentication & Access Control
Secure login with username and password
Role-based access control:
Admin: Full access to all features
Staff: Limited access (Sales and Customer management only)
Account locking after 3 consecutive failed attempts (5 minutes)
SHA-256 password hashing
Session management
✅ Inventory Management (Admin Only)
Add, edit, and delete medicines
Track stock quantities and reorder levels
Monitor expiry dates with alerts (30-day warning)
Low-stock alerts
Search and filter medicines by name, category, or batch number
✅ Sales & Billing
Create new sales transactions
Search and add medicines to cart
Calculate totals with discount support
Generate printable bills
Automatic inventory deduction after sale
✅ Customer Management
Add and manage customer records
Track purchase history
Search customers by name/phone
View customer spending patterns
✅ Supplier Management (Admin Only)
Add, edit, and delete supplier records
Store supplier contact information
Associate suppliers with medicines
Track supplier details
✅ Reports
Sales reports
Inventory reports
Expiry reports
Low stock reports
Export functionality
✅ Dashboard
Real-time statistics
Total medicines count
Low stock items alert
Medicines expiring soon
Today's sales summary
🛠️ Technology Stack
Component	Technology
Language	Java 11+
GUI Framework	Java Swing
Build Tool	Maven
Version Control	Git & GitHub
IDE	VS Code / Apache NetBeans
📁 Project Structure
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
🚀 Getting Started
Prerequisites
Java 11+ installed on your system
Maven 3.6+ installed
Git installed
VS Code with Extension Pack for Java (optional)
Installation & Running
Option 1: Using Maven (Command Line)
# Clone the repository
git clone https://github.com/iqra70735/pharmacy-management-system.git
cd pharmacy-management-system

# Build the project
mvn clean install

# Run the application
mvn exec:java -Dexec.mainClass="com.pharmacy.PharmacyApp"
Option 2: Using VS Code
Clone and open the project in VS Code
Install "Extension Pack for Java" from Extensions
Open terminal (Ctrl + `)
Run the commands from Option 1
Option 3: Create Executable JAR
mvn clean package
java -jar target/pharmacy-management-system-1.0.0.jar
👤 Test Credentials
Role	Username	Password
Admin	admin	admin123
Staff	staff	staff123
🎨 UI/UX Design
Color Scheme: Blue & White professional theme
Responsive Layout: Adapts to different screen sizes
Intuitive Navigation: Sidebar menu for easy access
Form Validation: Real-time input validation with error messages
Consistent Typography: Professional fonts throughout
Accessible Components: Easy-to-use buttons, tables, and fields
⚠️ Important Notes
Frontend Only: This is currently a frontend-only implementation. To integrate with a database:

Set up a database (SQLite, MySQL, or PostgreSQL)
Create database schema based on the models
Implement DAO/Repository layer
Update the UI components to use actual data from database
🔐 Security Features
✅ SHA-256 password hashing
✅ Account locking mechanism
✅ Session-based authentication
✅ Role-based access control
✅ Input validation

📱 Screenshots
(To be added)

🔄 Future Enhancements
 Database integration (SQLite/MySQL)
 Backend API integration
 Advanced reporting with charts/graphs
 Prescription management
 Multi-user support with detailed logging
 Email notifications
 Barcode scanning
 Mobile app version
📝 License
This project is open source and available under the MIT License.

👨‍💻 Author
Rabiya zainab

📞 Support
For issues, feature requests, or questions, please open an issue on GitHub.

Last Updated: January 2026
