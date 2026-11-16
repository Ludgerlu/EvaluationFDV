# Evaluation FDV

Evaluation FDV is a Laravel-based web application designed to manage and track employee performance evaluations across different organizational roles and services. The project provides role-based dashboards, evaluation forms, and reporting tools for administrative follow-up.

## Project overview

This application allows authorized users to:

- log in with their account and access a dedicated dashboard based on role
- create and review evaluation notes for staff members
- manage users, services, and regional assignments
- consult evaluation reports and final summaries
- monitor results by service, region, and evaluator type

The solution is organized around several user roles, including:

- CDS
- CDV
- CSC
- DR
- CDC TT
- Admin

Each category has specific routes and permissions, making the evaluation flow adapted to the structure of the organization.

## Main features

- Role-based authentication and access control
- User and service management
- Regional and functional assignment tracking
- Evaluation creation and review workflow
- Detailed reporting for each evaluated person
- Administrative dashboard for managing notes and results
- Password management and user profile access

## Technology stack

- PHP 8.1+
- Laravel 10
- Blade templates
- MySQL / database-driven persistence
- Bootstrap-based UI
- Artisan commands and Laravel middleware

## Project structure

- `app/Http/Controllers/` – controllers for authentication, dashboards, evaluations, and admin management
- `app/Models/` – data models such as users, notes, regions, and services
- `resources/views/` – Blade templates for the different role pages
- `routes/web.php` – main application routes and permission groups
- `database/migrations/` – database schema definitions
- `public/` – public assets and entry points

## Installation

1. Clone the repository.
2. Install PHP dependencies:

   ```bash
   composer install
   ```

3. Copy the environment file:

   ```bash
   cp .env.example .env
   ```

4. Generate the application key:

   ```bash
   php artisan key:generate
   ```

5. Configure your database connection in `.env`.
6. Run migrations and seeders if needed:

   ```bash
   php artisan migrate
   ```

7. Start the local server:

   ```bash
   php artisan serve
   ```

## Usage

After authentication, each user is redirected to the dashboard associated with their role. The application supports evaluations, notes handling, and report reviews according to the user profile.

## License

This project is licensed under the MIT License.
