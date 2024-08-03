# Basic Password Manager

This project is a simple password manager implemented in Python. It allows users to create accounts, store hashed passwords securely, and log in to their accounts. This project serves as an introductory exercise in cybersecurity and password management.

## Features

- **Account Creation**: Allows users to create new accounts with hashed passwords.
- **User Login**: Enables users to log in with their username and password.
- **Password Hashing**: Utilizes SHA-256 hashing to securely store passwords.
- **Data Persistence**: Saves user data to a file for persistence between runs.

## Prerequisites

- Python 3.x
- `hashlib` (included with Python)
- `getpass` (included with Python)
- `pickle` (included with Python)

## Installation

No additional installation is required beyond Python itself. Simply ensure you have Python 3.x installed on your system.

## Usage

1. **Run the Script**: Execute the Python script in your terminal or command prompt:
   ```sh
   python password_manager.py
   ```

2. **Menu Options**:
   - **Create Account**: Choose option `1` to create a new account. Enter a username and password when prompted.
   - **Login**: Choose option `2` to log in. Enter your username and password to access your account.
   - **Exit**: Choose option `0` to exit the application.

## Code Overview

- **`load_data()`**: Loads user data from the `user_data.pkl` file. Returns an empty dictionary if the file does not exist.
- **`save_data(data)`**: Saves user data to the `user_data.pkl` file.
- **`hash_password(password)`**: Hashes the provided password using SHA-256.
- **`create_account(user_data)`**: Prompts for username and password to create a new account. Stores the hashed password.
- **`login(user_data)`**: Prompts for username and password to log in. Verifies the provided password against the stored hash.
- **`main()`**: Displays a menu for user interaction. Handles account creation, login, and exits based on user input.

## Security Note

- Passwords are hashed using SHA-256 for storage. While this provides basic protection, for production systems, consider using more advanced hashing algorithms like bcrypt.
- Ensure the `user_data.pkl` file is stored securely to prevent unauthorized access.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

If you have suggestions or improvements for this project, please submit a pull request or open an issue on the GitHub repository.

## Contact

For any questions or feedback, please contact Karthik S Sathyan(karthikssathyan1@gmail.com).

