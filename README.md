# FeepaymentAlert_via_Email

# Admin Fee Notification System
#overview

This project is an administrative tool designed to manage user fee statuses and automate the process of sending email notifications. The application allows an admin to log in using OTP authentication and then perform several key actions such as updating fee statuses and sending out notifications to users with pending or cleared fees.

## Features

- **Admin Authentication**: Secure login with OTP verification.
- **User Management**: 
  - View and update fee payment statuses.
  - Maintain user details including name, email, and fee status.
- **Automated Email Notifications**:
  - Send emails to users with pending fee payments.
  - Send emails to users who have cleared their fees.

## Prerequisites

Before running the application, ensure you have the following:
- **Python 3.x** installed on your system.
- Custom modules (which must be available in your project or installed separately):
  - `feepending` – Module to handle sending emails to fee pending users.
  - `feepaid` – Module to handle sending emails to fee cleared users.
  - `otp` – Module to generate and send OTPs for admin authentication.

## Installation

pip install -r requirements.txt
Note: If feepending, feepaid, and otp are custom modules, ensure they are in your Python path or installed as needed.

Usage
Run the application by executing the main script:

python main.py
Workflow
Admin Login:

The script prompts for an admin username (expected username: admin).
An OTP is sent to the admin's registered email address. Enter the OTP to proceed.
Admin Options: Once logged in, the admin is presented with the following menu:

Edit Information: Update the fee status for each user (pending or cleared).
Send Mail to Fee Pending Users: Automatically send emails to users with a pending fee status.
Send Mail to Fee Cleared Users: Automatically send emails to users who have cleared their fees.
Exit: Exit the application.
Project Structure
graphql
Copy
Edit
.
├── main.py         # Main script that runs the admin tool
├── feepending.py   # Module for sending email notifications to fee pending users
├── feepaid.py      # Module for sending email notifications to fee cleared users
├── otp.py          # Module for OTP generation and sending
└── README.md       # This file
Note: Adjust the project structure as necessary to match your repository layout.

Contributing
Contributions are welcome! If you would like to contribute:

Fork the repository.
Create a new branch with a descriptive name.
Commit your changes.
Open a pull request for review.
