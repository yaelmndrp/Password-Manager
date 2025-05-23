# Password Manager

A secure and user-friendly password manager built with Python. This tool allows you to store, manage, and encrypt your passwords locally, ensuring your sensitive data is protected.

---

## Features

- **Secure Password Storage**: Passwords are encrypted using the Fernet encryption algorithm.
- **Master Password Protection**: A master password is required to access the password manager.
- **Password Strength Checker**: Ensures your passwords meet strong security requirements.
- **Random Password Generator**: Generates strong, random passwords that meet all security criteria.
- **Export Passwords**: Export your passwords to a file in either encrypted or plain-text format.
- **Expiry Tracking**: Automatically tracks password expiry dates (90 days by default).
- **User-Friendly Interface**: Simple command-line interface for easy navigation.

---

## Installation

1. **Clone the Repository**:

```bash
git clone https://github.com/S-Swayam/password-manager.git
cd password-manager
```

2. **Install Dependencies**:

Ensure you have Python 3.x installed, then install the required packages:
```bash
pip install -r requirements.txt
```

Then, run the Password Manager:

```
python password_manager.py
```

## Usage
### Setting Up the Master Password

When you run the program for the first time, you’ll be prompted to set up a master password. The master password must meet strong security requirements:

- At least 8 characters.
- Contains uppercase, lowercase, numbers, and special characters.

### Adding a Password
Choose the Add Password option from the main menu, enter the account name (e.g., Google, Facebook), username/email, and password.

You can either enter your own password or generate a strong, random one.

### Updating a Password
Select the Update Password option and enter the account name and provide a new username (optional) and password.

### Deleting a Password
Choose the Delete Password option and enter the account name and confirm the deletion.

### Listing Accounts
Use the List Accounts option to view all stored accounts and their usernames.

### Exporting Passwords
Select the Export Passwords option and choose a file name and decide whether to export in encrypted or plain-text format.

If exporting in plain-text, you’ll need to enter the master password for verification.

### Leaving the Program
Choose the Exit option to close the password manager.

### File Structure

| File path | Description |
| --------- | ----------- |
| /         | Root directory of the project |
| /data/    |Directory for storing sensitive files |
| /data/passwords.json | Encrypted password storage |
| /data/key.key | Encription key |
| /data/master_hash.txt | Master password hash |
| /data/password_manager.log | Log file |
| /password_manager.py | Main script |
| /README.md | This file |
| /requirements.txt | Dependencies |
| /LICENSE | License file |

### Security
- Encryption: Passwords are encrypted using the Fernet symmetric encryption algorithm.
- Master Password: The master password is hashed using bcrypt for secure storage.
- File Permissions: Sensitive files (e.g., key.key, passwords.json) are restricted to owner-only access.
- Logging: All actions are logged for auditing purposes.

### Requirements
Python 3.x

### Dependencies:

- bcrypt
- cryptography

**Install dependencies using:**
```bash
pip install -r requirements.txt
```

### Contributing
Contributions are welcome! If you’d like to contribute, please follow these steps:

- Fork the repository.
- Create a new branch for your feature or bugfix.
- Submit a pull request with a detailed description of your changes.

### License
This project is licensed under the MIT License. See the LICENSE file for details.

### Support
If you encounter any issues or have questions, feel free to open an issue on the GitHub repository.

Enjoy managing your passwords securely with this Password Manager! 🔒 
