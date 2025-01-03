# Mass SMTP Checker

**List Format**

 + domain.com|587|email@domain.com|password

**[ Description ]**

This tool is an SMTP checker designed to validate email accounts by attempting to log in to the specified SMTP servers with provided credentials. It processes a list of email account details in the format domain.com|587|email@domain.com|password from an input file. For each entry, it attempts to connect to the SMTP server, start a secure connection (if necessary), and log in using the given email and password.

If the login is successful, the tool logs the valid credentials into an output file. The script uses threading to speed up the process, checking multiple entries concurrently for faster results. It handles interruptions gracefully and prints status messages for each attempt, marking successful logins as [OK] and failures as [ERR].

**[ POV ]**

![alt text](https://raw.githubusercontent.com/cpkarma/img/refs/heads/main/smtp-checker/smtp.jpg)
