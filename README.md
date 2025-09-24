# 🚀 Student Books Borrowing - PHP & MySQL Environment + AutoWorld Car Website

A comprehensive development environment featuring a **PHP 8.1+** and **MySQL 8.0+** setup designed for **ICI students** using **GitHub Codespaces**, plus a complete automotive website showcasing modern web development techniques.

## 👨‍🎓 For ICI Students

### 📧 **Important: Use Your ICI Email Address**
Students should use their **ICI-email supplied email address** to use the privileges in the Codespace.

**Free Usage Limits:**
- **Free Accounts**: 120 hours per month
- **Verified Student/Teacher** (GitHub Student Developer Pack): **180 hours per month**
- Usage resets every month

## 🚗 AutoWorld Website Features

### Main Components
- **Car Reviews** - In-depth reviews of popular vehicle models
- **Latest News** - Automotive industry updates and announcements  
- **Buying Guide** - Comprehensive car purchasing advice
- **Maintenance Tips** - DIY guides and scheduled maintenance information
- **Car Gallery** - Interactive filterable showcase of different vehicle types

### Technical Features
- Responsive design optimized for all devices
- Modern CSS with smooth animations and transitions
- Interactive JavaScript functionality
- Mobile-friendly navigation with hamburger menu
- Gallery filtering system
- Smooth scrolling navigation
- Professional gradient design theme

## 🔧 PHP Development Environment

### Database Setup
- **Host:** mysql
- **Database:** basic_db  
- **Username:** root (or student)
- **Password:** root (or student)

### Available Tools
- **Database Testing** - `www/db-test.php`
- **CRUD Operations** - `www/simple-crud.php`  
- **PHP Information** - `www/phpinfo.php`
- **phpMyAdmin** - Available on port 8080
- **AutoWorld Website** - `www/cars.html`

## 📁 File Structure

```
/
├── .devcontainer/          # GitHub Codespaces configuration
├── config/                 # PHP and phpMyAdmin configuration
├── scripts/               # Setup and initialization scripts
└── www/                   # Web root directory
    ├── cars.html          # AutoWorld car website
    ├── cars.css           # Website styling
    ├── cars.js            # Interactive functionality
    ├── index.php          # Development environment homepage
    ├── db-test.php        # Database connection testing
    ├── simple-crud.php    # Basic CRUD operations demo
    └── phpinfo.php        # PHP configuration information
```

## 🚀 Getting Started

### View the Car Website
1. Open `www/cars.html` in your browser
2. Or navigate to `/cars.html` from the main index page

### PHP Development
1. Access the main environment at `www/index.php`
2. Test database connections with the provided tools
3. Use phpMyAdmin for database management
4. Create new PHP files in the www directory

## 🎨 AutoWorld Design Highlights

- **Color Scheme:** Professional blue/purple gradient theme
- **Typography:** Inter font for clean, modern appearance  
- **Layout:** Card-based design with hover effects
- **Icons:** FontAwesome integration for automotive themes
- **Responsiveness:** Mobile-first design approach

## 📱 Browser Compatibility

- Chrome/Chromium (recommended)
- Firefox
- Safari  
- Edge
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🛠️ Technologies Used

- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **Backend:** PHP 8.x
- **Database:** MySQL
- **Fonts:** Google Fonts (Inter)
- **Icons:** FontAwesome 6.4.0
- **Tools:** phpMyAdmin for database management

## 💻 Learning Examples

### 1. Basic Database Connection
```php
<?php
$conn = mysqli_connect("mysql", "root", "root", "basic_db");

// Check connection
if (!$conn) {
    die("Connection failed: " . mysqli_connect_error());
}
echo "Connected to database!";
mysqli_close($conn);
?>
```

### 2. Simple Query
```php
<?php
$conn = mysqli_connect("mysql", "root", "root", "basic_db");
$result = mysqli_query($conn, "SELECT * FROM users");
$users = mysqli_fetch_all($result, MYSQLI_ASSOC);

foreach ($users as $user) {
    echo $user['name'] . " - " . $user['email'] . "<br>";
}
mysqli_close($conn);
?>
```

## 🎯 What You Can Learn

### PHP Basics
- Variables and data types
- Control structures (if, for, while)
- Functions and arrays
- Form handling
- File inclusion

### Database Fundamentals
- Connecting to MySQL with MySQLi
- SELECT, INSERT, UPDATE, DELETE operations
- Prepared statements for security
- Basic database design

### Web Development
- HTML and PHP integration
- Processing form data
- Session management
- Basic security practices
- Modern responsive web design (AutoWorld example)

## 🚀 Quick Start / Setup

### 1. Create Your Environment
1. **Fork this repository** to your GitHub account (or use "Use this template")
2. **Click "Code" → "Create codespace on main"**
3. **Wait 2-3 minutes** for automatic setup
4. **Start coding!** Everything is ready to use

### 2. Access Your Environment

**🖥️ How to Access Your Application:**

1. **Wait for port forwarding** - VS Code will show port notifications
2. **Look for "Port 80" in the PORTS tab** at the bottom of VS Code
3. **Click the globe icon** 🌐 next to port 80 in the PORTS tab
4. **Or click "Open in Browser"** when the notification appears

## 🛠️ Development Workflow

1. **Write PHP code** in `www/` directory
2. **View your work** through port 80 forwarding (see PORTS tab)
3. **Manage database** with phpMyAdmin at `/phpmyadmin`
4. **Test connections** with the built-in test page
5. **Save your work** using Git (commit and push regularly)

## 🐛 Troubleshooting

### 🌐 Can't Access Your Website?
- **Wait for port forwarding**: Look for notifications about port 80 being forwarded
- **Check PORTS tab**: Click the PORTS tab at the bottom of VS Code
- **Click the globe icon** 🌐 next to port 80

### 🗄️ Database Connection Issues?
- **Use `mysql` as host** (NOT `localhost`!)
- **Wait for MySQL to fully start** (can take 1-2 minutes)
- **Check credentials**: `root/root` or `student/student`
- **Verify database name**: `basic_db`

### 🛠️ phpMyAdmin Access
1. **Open your main website** in the browser (Port 80)
2. **Add `/phpmyadmin`** to the end of your URL
3. **Login**: Username: `root`, Password: `root`

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

---

**Student Books Borrowing Environment** - Complete PHP/MySQL learning environment with AutoWorld car website example | Built for ICI students 💻✨