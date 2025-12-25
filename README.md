```
____                                     _            _   _            
|  _ \ __ _ ___ _____      _____  _ __ __| |  ___  ___| |_| |_ ___ _ __ 
| |_) / _` / __/ __\ \ /\ / / _ \| '__/ _` | / __|/ _ \ __| __/ _ \ '__|
|  __/ (_| \__ \__ \\ V  V / (_) | | | (_| | \__ \  __/ |_| ||  __/ |   
|_|   \__,_|___/___/ \_/\_/ \___/|_|  \__,_| |___/\___|\__|\__\___|_|   

```
This is a sloppy Python project to train myself to password inputs and handling hashes.
This is not meant to be used in production.
PAsswords will be hashed in sha-256 and stored in a dedicated user.db SQL database. Please ensure to safely store it
It probably sucks and if by any chance to read this please feel free to tell me how to improve it.

# Features
- Register users with a unique username and password
- Verify passwords against stored hashes
- Store data securely in a SQLite database (users.db)
- Basic error handling for database operations

# Requirements
- Python 3.6+
- Standard Python modules: getpass, hashlib, sqlite3

# Installation
- Clone or download the source code
- Ensure Python 3 is installed: python3 --version
- Navigate to the directory containing main.py

# Usage
Run the script: python3 main.py
Follow prompts:Enter a username
- Set and confirm a password
- If the username is unique, it’s saved to users.db
- Enter the password again to verify access

# Database Structure
Table users:username (TEXT, primary key): Unique username.
password hash (TEXT, not null): SHA-256 pasword hash

(real nerds listen to UwU_underground)
