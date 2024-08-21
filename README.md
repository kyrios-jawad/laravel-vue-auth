# Laravel Vue.js Authentication Application

This project is a simple web application that provides basic user authentication (login and registration) using Laravel as the backend framework and Vue.js for the frontend. The project is designed with a focus on simplicity and ease of use, implementing form validation and error handling.

## Table of Contents

- [Technologies Used](#technologies-used)
- [Features](#features)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [License](#license)

## Technologies Used

- **PHP**: Backend programming language.
- **Laravel**: PHP framework for building web applications.
- **Vue.js**: JavaScript framework for building interactive user interfaces.
- **Vite**: Frontend build tool used by Laravel for bundling assets.
- **Tailwind CSS**: Utility-first CSS framework used for styling.
- **Laravel Breeze**: Provides minimal and simple authentication functionality for Laravel applications.
- **Inertia.js**: Allows for server-side rendering with Vue.js, providing a single-page application experience.

## Features

- User registration and login.
- Form validation with meaningful error messages.
- SPA-like experience with Vue.js.
- Simple and clean design using Tailwind CSS.

## Installation

### Prerequisites

- **PHP >= 8.1**
- **Composer**
- **Node.js >= 16.x**
- **NPM or Yarn**
- **MySQL or any other supported database**

### Clone the Repository

```bash
git clone https://github.com/your-username/laravel-vue-auth.git
cd laravel-vue-auth
```

Setup Backend (Laravel)
Install Dependencies:

```bash
composer install
```
Environment Configuration:

Copy the .env.example file to .env and configure your database connection and other environment variables:

```bash
cp .env.example .env
```
Update the .env file:

APP_NAME="Laravel Vue Auth"
APP_URL=http://127.0.0.1:8000
DB_DATABASE=your_database_name
DB_USERNAME=your_database_user
DB_PASSWORD=your_database_password
Generate Application Key:

```bash
php artisan key:generate
```
Run Migrations:

```bash
php artisan migrate
```
Setup Frontend (Vue.js)
Install Node Dependencies:

```bash
npm install
```
Compile Assets:

```bash
npm run dev
```

Running the Application
Start the Laravel Development Server:

```bash
php artisan serve
```
The application will be available at http://127.0.0.1:8000.

Visit the Login or Registration Page:

For login: http://127.0.0.1:8000/login
For registration: http://127.0.0.1:8000/register
Project Structure
The project follows the standard Laravel structure with Vue.js components integrated via Laravel Breeze.

app/: Contains the core logic of the application.
resources/views/: Contains Blade templates and Vue.js components.
routes/web.php: Defines the web routes for the application.
resources/js/Pages/: Contains Vue.js pages for login and registration.
resources/css/: Tailwind CSS configuration.
public/: Publicly accessible assets like images and compiled CSS/JS.
database/migrations/: Contains migration files to set up the database schema