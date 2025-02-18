# Bulk-Mail-CSV

This Python script sends bulk emails to recipients listed in a CSV file. It uses the `smtplib` library to connect to an SMTP server and send emails.

## Prerequisites

- Python 3.x
- `smtplib` library
- `csv` library
- `email` library

## Files

- `main.py`: Main script to send emails
- `credentials.txt`: Contains email address and password
- `emails.csv`: List of recipient email addresses

## Usage

1. Clone the repository:

```bash
git clone https://github.com/shreyash0019/Bulk-Mail-CSV.git
```
2. Navigate to the project directory:
  ```bash
 cd Bulk-Mail-CSV
 ```
4. Install the required libraries:
``` bash
pip install smtplib email csv
```
5. Create a credentials.txt file in the project directory with the following format:
```bash
 your_email@example.com
 your_password ```
```
6. Run the script:
   ``` bash
   python main.py
```
```
Script Explanation
The script performs the following steps:

1. Reads the email credentials from credentials.txt.

2. Logs in to the SMTP server.

3. Reads the recipient email addresses from emails.csv.

4. Sends the email to each recipient.



