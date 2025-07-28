# 🛠 UrbanServe – Local Service Management System

UrbanServe is a PHP & MySQL-based platform designed to connect customers with service providers for a variety of local services. It features role-based dashboards for Admins, Service Providers, and Customers, and supports a complete booking, profile, and verification workflow.

---

## 📁 Project Structure

```
localservice-main/
├── about.php                    # About Us page
├── add_service.php             # Form for providers to add new services
├── admin_dashboard.php         # Admin panel overview
├── bookings.php                # Booking management for all users
├── book_service.php            # Service booking page (customer side)
├── contact.php                 # Contact Us page
├── customer_bookings.php       # Customer's booking history
├── customer_dashboard.php      # Dashboard for customers
├── db.php                      # Database connection script
├── edit_my_services.php        # Providers edit their own services
├── edit_profile.php            # Profile update page for all roles
├── edit_services.php           # Admin edits any provider's services
├── index.php                   # Homepage
├── login.php                   # Login page
├── logout.php                  # Logout handler
├── manage_categories.php       # Admin manages service categories
├── my_bookings.php             # Provider's booking view
├── providers.php               # Public listing of service providers
├── provider_bookings.php       # Booking list for providers
├── provider_dashboard.php      # Provider dashboard
├── provider_profile.php        # Public profile of a provider
├── register.php                # User registration page
├── services.php                # Browse services with filters
├── service_detail.php          # Detailed view of a service
├── upload_id_proof.php         # Providers upload ID for verification
├── users.php                   # Admin user list
├── view_booking.php            # View full booking detail
├── view_id_proof.php           # Admin reviews uploaded ID proof
├── urbanserve.sql              # MySQL database structure and seed data
```

---

## 🧑‍💼 Roles & Features

### 👤 Admin

* Manage users and providers
* Approve or reject provider ID verification
* Edit or delete services and categories

### 🧰 Service Provider

* Add/edit services they offer
* View/manage customer bookings
* Update profile including experience, bio, location
* Upload ID proof for verification

### 🧍 Customer

* Browse services by category, location, and rating
* Book services and view booking history
* Manage their own profile

---

## 🛠 Setup Instructions

### Requirements

* PHP 7.x or higher
* MySQL 5.7 or higher
* Apache Server (XAMPP/LAMP/WAMP)

### Steps

2. **Move the folder to your web server root**

   * Example for XAMPP: `C:/xampp/htdocs/localservice-main`

3. **Import the database**

   * Open `phpMyAdmin`
   * Create a new database named `urbanserve`
   * Import the `urbanserve.sql` file

4. **Configure database**

   * Open `db.php`
   * Update credentials if needed:

     ```php
     $conn = new mysqli("localhost", "root", "", "urbanserve");
     ```

5. **Run in browser**

   * Visit: `http://localhost/localservice-main/`

---

## ✅ Notes

* No online payment integration is included.
* Image upload is available for provider ID proof only.
* Pages use basic PHP and MySQLi (no frameworks).

---

## 📞 Contact

For support or improvements, reach out at: \[[your-email@example.com](mailto:your-email@example.com)]

---
