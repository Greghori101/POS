## Point Of Sale multilanguage (English - Arabic)

# Laravel 8 Project Setup

Follow these steps to set up and run the project locally using **PHP 8.0**.

## ✅ Requirements

- **PHP 8.0**
- **Composer**
- **MySQL**
- **Node.js and NPM** (optional, for front-end assets)

## 🚀 Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone <your-repo-url>
   cd <project-directory>
   ```

2. **Install PHP Dependencies**

   Ensure you're running **PHP 8.0**, then install dependencies:

   ```bash
   composer install
   ```

3. **Copy `.env` File**

   ```bash
   cp .env.example .env
   ```

4. **Configure Environment Variables**

   Open the `.env` file and set the necessary values:

   ```env
   APP_NAME=Laravel
   APP_ENV=local
   APP_KEY=
   APP_DEBUG=true
   APP_URL=http://localhost:8000

   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=your_database_name
   DB_USERNAME=your_database_user
   DB_PASSWORD=your_database_password
   ```

5. **Generate Application Key**

   ```bash
   php artisan key:generate
   ```

6. **Run Migrations**

   ```bash
   php artisan migrate
   ```

7. **Insert Example Data**

   If you have a SQL script for sample data:

   ```bash
   mysql -u your_database_user -p your_database_name < ./db_files/my-pos.sql
   ```

8. **Start the Development Server**

   ```bash
   php artisan serve
   ```

   Then open [http://localhost:8000](http://localhost:8000) in your browser.
