# Password Reset Application

This Python script enables users to securely reset their passwords.

## Features

Username verification: Ensures the user exists in the database.
Security question verification: Adds an extra layer of authentication.
Strong token generation: Uses secure random tokens for password resets.
Token expiration: Prevents unauthorized access after a specified time.
Email-based password reset: Sends a password reset link to the user's email.
Password strength validation: Enforces password complexity requirements.
Error logging: Records errors for debugging purposes.
## Requirements

Python 3.x
psycopg2 (for PostgreSQL database interaction)
smtplib (for sending emails)
secrets (for secure token generation)
## Setup

Install required libraries: pip install psycopg2 smtplib secrets
Replace placeholders in the code with your actual:
Database credentials
Email server settings
URL for password reset
Preferred password hashing algorithm (e.g., bcrypt)
## Usage

Run the script: python password_reset.py
Follow the prompts to initiate a password reset.
## Security Considerations

Input validation: Implement robust input validation to prevent injection attacks.
Password hashing: Always store passwords using a secure hashing algorithm.
Secure database interactions: Use parameterized queries to avoid SQL injection vulnerabilities.
