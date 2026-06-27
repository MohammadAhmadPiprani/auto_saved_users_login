
# User-login-monitor

A Bash shell script engineered for system administration and auditing purposes. It prompts an interactive user login session, tracks active users, and logs historical session metadata directly to a structured log file.

This tool acts as a lightweight security utility to maintain a verifiable audit trail of user access on Linux environments.

## 🚀 Key Features

* **Automated Time-Stamping:** Automatically records the exact execution execution time using native Linux `date` utilities.
* **Active User Identification:** If no username is specified, it leverages the `who` command to capture a snapshot of all currently active terminal sessions.
* **Historical Auditing:** Leverages the `last` utility and pipes it into `head` to capture and store the specific user's last two authentication records.
* **Persistent Output Tracking:** Saves all processed data into a dedicated `login.txt` audit file for persistence.

## 📦 Script Logic Workflow
