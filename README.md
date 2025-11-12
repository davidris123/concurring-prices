# Concurring-Prices

## Description
A simple PHP laravel app intended to showcase the different prices of products in stores across Macedonia.

## Screenshot
![Homepage](images/image.png)

---

## Prerequisites

Ensure you have the following software installed on your machine:

- **PHP** (for Laravel framework)
- **Composer** (for managing PHP dependencies)
- **Python 3.x** (for running Python scripts)
- **pip** (Python package manager)
- **Virtualenv** (for Python virtual environment)

Additionally, ensure that you have a working MySQL database setup for Laravel migrations. The database should be named concurringprices and it contains the default username & password for the server

---

## Installation Instructions

Follow the steps below to set up and run the project:

### 1. Install PHP Dependencies

Start by installing the required PHP dependencies using Composer:

```bash
composer install
```

### 2. Set Up Python Virtual Environment

Create a Python virtual environment to isolate your project’s dependencies:

For Windows & Mac/Linux:

```bash
py -m venv venv
```

### 3.1 Activate the Virtual Environment

To activate the virtual environment:

#### For Windows (Command Prompt):
```bash
cd venv\Scripts
activate
```

#### For Windows (Powershell):
```bash
cd venv\Scripts
./activate
```

#### For Unix/macOS
```bash
source venv/bin/activate
```

### 3.2 Install Python Dependencies

With the virtual environment activated, return to the root directory and install the necessary Python dependencies by running:

```bash
cd ../..
pip install -r requirements.txt
```

## 3.3 (Optional) Run the scraper 

As to not wait the scheduled day for the scraper to run, you can run it immediately.
While venv is still activated, run the scraper from the root directory:
```bash
python .\scripts\scraper.py
```

### 4. Run the Laravel Migrations

To set up your database and run the necessary migrations, use the following command:

```bash
php artisan migrate
```

### 6. Generate App Key & Run the Development Server

```bash
php artisan key:generate
php artisan serve
```

### 7. (Optional) Schedule the job

To schedule the job, use the following command

```bash
php artisan schedule:work
```
