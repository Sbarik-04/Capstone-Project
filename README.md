# Capstone-Project
# 💬 Feedback Form Web App

This is a Capstone Project for the **Web Technology Lab**. It’s a modern feedback collection system built with **HTML**, **CSS**, **PHP**, and **MySQL** (via phpMyAdmin). A `.txt` file serves as a backup for all submitted feedback.

## 🚀 Features

- Responsive web UI
- Collects Name, Email, Rating, and Comments
- Stores feedback in a MySQL database using PHP
- Backup to `feedbacks.txt`
- Thank-you page after successful submission

## 🧰 Technologies Used

- **Frontend:** HTML5, CSS3, Google Fonts, Font Awesome
- **Backend:** PHP
- **Database:** MySQL (via phpMyAdmin)
- **Backup:** Plain text log (feedbacks.txt)

## 📂 Project Structure
├── index.html # Frontend form
├── style.css # Stylesheet
├── process_feedback.php # PHP logic for handling form submission
├── thankyou.html # Acknowledgment page
├── feedbacks.txt # Backup of submitted feedbacks
├── sql/ # Contains .sql file for feedbacks table (exported)

## 🧾 Database Setup

1. Open **phpMyAdmin**
2. Create a new database, e.g., `feedback_system`
3. Import `feedbacks.sql` from the `sql/` directory
4. Ensure your database credentials in `process_feedback.php` are correct

**SQL Table Structure:**
```sql
CREATE TABLE `feedbacks` (
  `id` INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `name` VARCHAR(100),
  `email` VARCHAR(100),
  `rating` INT,
  `comments` TEXT,
  `submitted_at` TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```
**Running the Project**
Install XAMPP

Start Apache and MySQL

Place all files into htdocs/your-folder-name/

Open browser and visit: http://localhost/your-folder-name/index.html

