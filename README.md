# 🚍 MTC Accounts & Audit Management System
# Project Overview

This web application is a specialized ERP (Enterprise Resource Planning) tool developed for the Metropolitan Transport Corporation (Chennai) Ltd. It is designed to streamline the auditing process, manage employee master data, and generate detailed ticket inventory and financial reports across various depots.

The system provides a secure, centralized platform for the Accounts department to monitor stock levels, track employee records, and ensure financial transparency within the corporation.
## ✨ Key Features

    Secure Employee Authentication: A dedicated login portal for authorized personnel to access sensitive audit data.

    Employee Master Management: A lookup system using EDP Numbers to manage and verify employee credentials and details.

    Depot-wise Audit Reporting: Comprehensive reporting modules for various depots (e.g., Alanthur, Ambattur, Anna Nagar) that track:

        Regular Stock & Tray Stock

        Monthly Season Tickets (MST)

        TAYPT and SCT/SMT data

    Automated Calculations: Real-time totals and data aggregation for inventory and accounting audits.

    Responsive Dashboard: A clean, professional user interface designed for high-density data entry and analysis.

## 🛠️ Tech Stack

    Frontend: HTML5, CSS3, JavaScript (with a focus on data-heavy tables and modal interactions).

    Backend: PHP (handling server-side logic and session management).

    Database: Likely MySQL/MariaDB (for storing employee master records and audit logs).

## 🚀 Getting Started

To run this application locally for development or testing, you will need a local PHP environment.
Prerequisites

    XAMPP / WAMP / MAMP: A local server environment containing Apache and MySQL.

    Web Browser: Chrome, Firefox, or Edge.

    Code Editor: VS Code or similar.

## Installation & Setup

    Clone the Repository
    Bash

    git clone https://github.com/your-username/mtc-audit-system.git

    Move to Local Server Directory

        If using XAMPP: Move the project folder to C:/xampp/htdocs/

        If using WAMP: Move the project folder to C:/wamp64/www/

## Database Configuration

        Open phpMyAdmin (http://localhost/phpmyadmin).

        Create a new database named mtc_audit.

        Import the database.sql file (if provided) from the root directory of this project.

## Connect the Database

        Open config.php or db_connect.php (or wherever your connection logic lives).

        Update the credentials to match your local setup:
        PHP

        $servername = "localhost";
        $username = "root";
        $password = ""; // Default XAMPP password is empty
        $dbname = "mtc_audit";

## Run the Application

        Start Apache and MySQL in your XAMPP/WAMP control panel.

        Open your browser and navigate to:
        http://localhost/mtc-audit-system/login.php

## 🛠️ Project Structure

    /audit/ - Contains the core application files.

    login.php - Secure entry point for employees.

    empcheck.php - Employee master data validation module.

    ticketreportnew.php - Main reporting engine for depot audits.

A small tip for your GitHub repo:

Make sure you include a .gitignore file! You don't want to accidentally push your local database passwords or temporary server logs to the public internet.
