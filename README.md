# OTP Verification Using Python with Email

This project demonstrates how to implement OTP (One-Time Password) verification using Python and email. OTP verification is commonly used in applications to authenticate users and ensure the security of sensitive operations.

## Prerequisites

To run this project, you need the following:

1. Python (version 3.6 or later)
2. SMTP server details (for sending emails)

## Installation

1. Clone this repository or download the source code.
2. Open a terminal or command prompt and navigate to the project directory.
3. Install the required dependencies by copying the code from import section.

  
## Configuration

Before running the project, you need to configure the following:

1. SMTP server details: Open the `config.py` file and enter the details of your SMTP server, such as host, port, username, and password.

   ```python
   # SMTP server configuration
   SMTP_SERVER = 'your_smtp_server_host'
   SMTP_PORT = your_smtp_server_port
   SMTP_USERNAME = 'your_smtp_username'     i.e your email id
   SMTP_PASSWORD = 'your_smtp_password'     i.e your email password
   ```

2. Sender and recipient email addresses: In the `otp_verification.py` file, update the `sender_email` and `receiver_email` variables with the appropriate email addresses.

   ```python
   # Email addresses
   sender_email = 'your_sender_email@example.com'
   receiver_email = 'your_recipient_email@example.com'
   ```

## Usage

To run the OTP verification process, follow these steps:

1. Open a terminal or command prompt and navigate to the project directory.
2. Run the following command:

   ```
   python otp_verification.py
   ```

3. The program will generate a random OTP and send it to the specified email address.
4. Check your email inbox and note down the received OTP.
5. Enter the OTP in the terminal or command prompt when prompted.
6. The program will validate the entered OTP and display a success message if it matches.

## Customization

You can customize the OTP length, email subject, and email content by modifying the `otp_verification.py` file. Look for the following variables and update them according to your requirements:

- 'otp_length'
- `email_subjects`: The subject line of the verification email
- `email_body`: The content of the verification email

## Conclusion

This project provides a simple implementation of OTP verification using Python and email. You can integrate this code into your applications to add an extra layer of security to user authentication and sensitive operations. Feel free to modify and enhance the code as per your specific requirements.
