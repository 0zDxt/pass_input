```
____                                     _            _   _            
|  _ \ __ _ ___ _____      _____  _ __ __| |  ___  ___| |_| |_ ___ _ __ 
| |_) / _` / __/ __\ \ /\ / / _ \| '__/ _` | / __|/ _ \ __| __/ _ \ '__|
|  __/ (_| \__ \__ \\ V  V / (_) | | | (_| | \__ \  __/ |_| ||  __/ |   
|_|   \__,_|___/___/ \_/\_/ \___/|_|  \__,_| |___/\___|\__|\__\___|_|   

```
This Python program enables user registration and authentication by storing usernames and hashed passwords in a SQLite database. It uses SHA-256 for password hashing and provides a command-line interface.

# Features
- Register users with a unique username and password.
- Verify passwords against stored hashes.
- Store data securely in a SQLite database (users.db).
- Basic error handling for database operations.

# Requirements
- Python 3.6+
- Standard Python modules: getpass, hashlib, sqlite3

No additional dependencies required.

# Installation
- Clone or download the source code.
- Ensure Python 3 is installed: python3 --version.
- Navigate to the directory containing main.py.

# Usage
Run the program: python3 main.py
Follow prompts:Enter a username.
- Set and confirm a password.
- If the username is unique, it’s saved to users.db.
- Enter the password again to verify access.

# Project Structure
main.py: Main script for user registration and authentication.
users.db: SQLite database storing usernames and password hashes.

# Database Structure
Table users:username (TEXT, primary key): Unique username.
password hash (TEXT, not null): SHA-256 password hash.

# Security
Passwords are hashed with SHA-256.
Ensure users.db is stored securely with restricted permissions.
