# Linux-User-Management-Automation-CLI
A fully featured Bash script for automating user creation, group assignment, home directory setup, sudo permissions, password complexity enforcement, and account expiration—all driven via CSV batch input or interactive prompts.



## 📌 Features


✅ Batch user creation via CSV

👥 Automatic group handling

🏠 Secure home directory setup

🔐 Password complexity enforcement

🛡️ Optional sudo permission assignment

📅 Account expiration date support

🧾 Logs activities to /var/log/user_cli.log

🧠 Fallback interactive mode if no CSV provided



## 🚀 Usage
### 🔧 Step 1: Make Script Executable
bash
chmod +x user_cli.sh

### 📦 Step 2: Run in Batch Mode
bash
sudo ./user_cli.sh users.csv

### 🧑‍💻 Step 3: Run in Interactive Mode (if no CSV)
bash
sudo ./user_cli.sh
The script will prompt for username, password, group, sudo access, and expiration date.

#### 📝 Logging
All operations and validations are recorded to:

/var/log/user_cli.log
This includes:

Group creation notices

User creation success/failure

Password validation errors

Sudo assignment logs

Home folder setup status

#### 🔒 Password Policy
The script enforces:

Minimum 8 characters

At least one uppercase letter

At least one digit

Weak passwords are rejected and skipped during execution.

#### 📅 Account Expiration
Each user account can be assigned an expiration date (format: YYYY-MM-DD). This ensures:

Temporary access provisioning

Automated lockout after the deadline

Easier compliance in secure environments

#### ⚙️ Extensibility Ideas
Future improvements:

🔔 Email notifications for new accounts

📊 Summary reports or dashboards

🧑‍💼 Role-based permission templates

🌐 GUI front-end via Zenity or Tkinter

🔍 Audit tools with cron scheduling


#### 💼 Portfolio Value
This project demonstrates:

Linux system administration and scripting

Security-conscious design (passwords, access control)

Automation pipelines using CSV and shell logic

Error handling, input validation, and interactive UX

Logging and audit capabilities
