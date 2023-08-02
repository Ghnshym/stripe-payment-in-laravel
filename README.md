
# Stripe Payment Integration with Laravel

This is a simple Laravel web application that demonstrates the integration of Stripe payment for processing card payments. Users can make test payments using the provided test card details.

## Prerequisites

Before you begin, make sure you have the following installed on your local machine:

- [Composer](https://getcomposer.org/) - Dependency manager for PHP
- [PHP](https://www.php.net/) - Version 7.3 or higher
- [MySQL](https://www.mysql.com/) or [SQLite](https://www.sqlite.org/index.html) - Database system
- [Stripe Account](https://stripe.com/) - To obtain API keys

## Getting Started

Follow the steps below to get the project up and running on your local machine:

### 1. Clone or Download the Repository

To clone the repository, open your terminal or command prompt and run:

```bash
git clone https://github.com/Ghnshym/stripe-payment-in-laravel.git
```

Alternatively, you can download the ZIP file by clicking on the "Code" button on the repository page and selecting "Download ZIP."

### 2. Install Dependencies

Navigate to the project directory and install the project dependencies using Composer:

```bash
cd stripe-payment-in-laravel
composer install
```

### 3. Configure Environment Variables

Rename the `.env.example` file to `.env`:

```bash
cp .env.example .env
```

Open the `.env` file in a text editor and set the following environment variables:

```ini
APP_NAME=StripePayment
APP_ENV=local
APP_KEY=your-random-key
APP_DEBUG=true
APP_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your-database-name
DB_USERNAME=your-database-username
DB_PASSWORD=your-database-password

STRIPE_KEY=your-stripe-publishable-key
STRIPE_SECRET=your-stripe-secret-key
```

Replace `your-random-key`, `your-database-name`, `your-database-username`, `your-database-password`, `your-stripe-publishable-key`, and `your-stripe-secret-key` with your actual values.

You can generate `APP_KEY` using this artisan :

```bash
php artisan key:generate
```

### 4. Migrate Database

Run the database migrations to create the required tables:

```bash
php artisan migrate
```

### 5. Serve the Application

You can use the built-in development server to run the application:

```bash
php artisan serve
```

The application will be available at `http://localhost:8000/stripe`.


## Testing Stripe Payment

To test the Stripe payment integration, use the following test card details:

- Card Number: 4242 4242 4242 4242
- Expiry Date (MM/YY): 04/25
- CVC: 005
- ZIP: 55555

Please note that these are test card details meant for demonstration purposes only. In a real production environment, you would need to use valid card information.

```
Thank You for Visiting Here :)) Happy Coding😊 
