# Your Reliever

**Your Reliever** is a well-being companion web application designed to help individuals, particularly campus students, manage stress and anxiety. It achieves this through guided content, practical tools, and access to supportive communities and licensed professionals.

## 🚀 Features

- **Mindful Relief (Content Library):** Access guided breathing, meditation exercises, and tips specifically curated for mental wellness.
- **Professional Support (Book Professional):** Connect and book sessions securely with licensed mental health professionals.
- **Community Care (Chat Forum):** Join a supportive, moderated discussion community where members can share experiences and encourage one another safely.
- **Stress & Anxiety Education:** Learn about the differences between stress, anxiety, and depression, along with actionable coping mechanisms.
- **Emergency Support:** Quick, reliable access to emergency contacts and support networks.

## 🛠️ Technology Stack

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Backend:** PHP (Custom API and Models)
- **Database:** MySQL / MariaDB

## 📋 Prerequisites

To run this project locally, you will need:
- A local server environment such as **XAMPP**, **WAMP**, or **MAMP** (which include Apache and MySQL).
- A modern web browser (Chrome, Firefox, Edge, Safari).

## ⚙️ Installation & Setup

1. **Clone or Download the Repository:**
   Place the project folder (`YourReliever`) into your local server's web root directory:
   - For XAMPP: `C:/xampp/htdocs/YourReliever`
   - For WAMP: `C:/wamp/www/YourReliever`

2. **Database Setup:**
   - Open **phpMyAdmin** (usually accessible at `http://localhost/phpmyadmin`) or your preferred MySQL client.
   - Create a new database named `yourreliever`.
   - Import the database schema by executing the SQL script found at `backend/Database/schema.sql`.
   - *(Optional)* Import the sample data by executing `backend/Database/Your Reliever insertions.sql`.

3. **Database Configuration:**
   - Open the file `backend/config.php`.
   - Check the database credentials. By default, it expects user `root` with no password (`''`). If your local database uses a different user or password, update them here:
     ```php
     'db' => [
       'host' => '127.0.0.1',
       'port' => 3306,
       'name' => 'yourreliever',
       'user' => 'root',   // Update if necessary
       'pass' => '',       // Update if necessary
       'charset' => 'utf8mb4'
     ]
     ```

4. **Run the Application:**
   - Start the **Apache** and **MySQL** services in your local server control panel.
   - Open your web browser and navigate to the project:
     `http://localhost/YourReliever/Index.html`
     *(Adjust the URL path depending on the exact folder structure inside your web root).*

## 📂 Project Structure

```text
YourReliever/
├── Index.html                  # Main landing page
├── *.html, *.css, *.js         # Frontend pages, stylesheets, and scripts
├── Images/                     # Image assets and icons
├── SlideShow/                  # Images for the homepage carousel
├── Media/ & video/             # Additional media resources
└── backend/                    # PHP backend directory
    ├── config.php              # Global configuration and DB credentials
    ├── bootstrap.php           # App initialization
    ├── connection.php          # Database connection handler
    ├── api/                    # API route endpoints
    ├── models/                 # PHP Data models
    └── Database/               # SQL scripts for database schema and sample data
```

## 👨‍💻 Development Team

This project was developed by a passionate team of developers from the Faculty of Computing and Informatics at **Mbarara University of Science and Technology (MUST)**, Uganda:

- Nsubuga Arafat
- Mwima Edrine
- Ngabirano Haniel
- Natukunda Mary Ritah
- Namanya Spencar

## 📜 License

&copy; 2025 YourReliever. All Rights Reserved.
