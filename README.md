# Laravel Project Setup  

## Prerequisites  

Before setting up the Laravel project, ensure you have the following installed on your system:  

- **PHP** (version 8.0 or later) → [Download PHP](https://www.php.net/downloads.php)  
- **Composer** (Dependency Manager for PHP) → [Get Composer](https://getcomposer.org/)  
- **Node.js & npm** (For frontend assets, optional) → [Download Node.js](https://nodejs.org/)  
- **Database** (MySQL, PostgreSQL, SQLite, or MongoDB as per your preference)  

## Installation Steps  

### 1. Clone the Project Repository  

```bash
git clone https://github.com/your-repository-name.git
cd your-repository-name
2. Install Dependencies
Run the following command to install PHP dependencies:
composer install
If your project requires frontend assets, install npm dependencies:

sh
Copy
Edit
npm install
3. Configure Environment File
Copy the example environment file and update it with your database credentials:

sh
Copy
Edit
cp .env.example .env
Now, open the .env file and configure your database settings:

env
Copy
Edit
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_user
DB_PASSWORD=your_database_password
4. Generate Application Key
Run the command below to generate an application key:

sh
Copy
Edit
php artisan key:generate
5. Run Database Migrations
Execute the following command to create database tables:

sh
Copy
Edit
php artisan migrate
6. Start the Development Server
Launch the Laravel application using:

sh
Copy
Edit
php artisan serve
Your application will now be accessible at:

cpp
Copy
Edit
http://127.0.0.1:8000
7. Compile Frontend Assets (Optional)
If your project includes frontend assets using Laravel Mix or Vite, run:

sh
Copy
Edit
npm run dev
8. Running Tests (Optional)
To run automated tests, execute:

sh
Copy
Edit
php artisan test
Additional Commands
Clear Cache →
sh
Copy
Edit
php artisan cache:clear
Migrate with Fresh Data →
sh
Copy
Edit
php artisan migrate:fresh --seed
Storage Link (For file uploads) →
sh
Copy
Edit
php artisan storage:link
Deployment
For deploying your Laravel application to a production server, refer to the Laravel Deployment Guide.
