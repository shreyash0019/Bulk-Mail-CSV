# Bulk-Mail-CSV

This Python script sends bulk emails to recipients listed in a CSV file. It uses the `smtplib` library to connect to an SMTP server and send emails.

## Prerequisites

- Python 3.x
- Standard libraries (`smtplib`, `csv`, and `email`) are included with Python.

## Files

- `main.py`: Main script to send emails.
- `credentials.txt`: Contains email address and password.
- `emails.csv`: List of recipient email addresses.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/shreyash0019/Bulk-Mail-CSV.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Bulk-Mail-CSV
   ```

3. Ensure Python is installed on your system.

4. Create a `credentials.txt` file in the project directory with the following format:

   ```text
   your_email@example.com
   your_password
   ```

5. Ensure you have an `emails.csv` file with the following format (column name optional):

   ```csv
   email
   recipient1@example.com
   recipient2@example.com
   recipient3@example.com
   ```

6. Run the script:

   ```bash
   python main.py
   ```

## Script Explanation

The script performs the following steps:

1. Reads the email credentials from `credentials.txt`.
2. Logs in to the SMTP server.
3. Reads the recipient email addresses from `emails.csv`.
4. Sends the email to each recipient.

### Notes:

- Ensure that your SMTP server settings are correct (e.g., `smtp.gmail.com` for Gmail).
- Some email services may block login attempts from less secure apps. You may need to enable "less secure app access" or generate an app password.
- For better security, avoid hardcoding credentials directly in the script.

## Troubleshooting

- **Authentication Errors**: Ensure credentials are correct and not blocked by the email provider.
- **Connection Errors**: Check your internet connection and SMTP server settings.
- **Email Delivery Issues**: Verify that recipient email addresses are valid and not flagged as spam.

Feel free to modify the script to suit your needs and add features like custom email subjects, body content, or attachments.



