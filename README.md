# Ansible System Setup

This project uses Ansible to automate system setup for **web** and **database** servers.  
It installs required packages, creates users, and deploys configuration files.

---

## Project Structure

├── site.yml # Main playbook
├── inventory.ini # Inventory with server details
├── roles/
│ └── system_setup/
│ ├── tasks/main.yml # Main tasks
│ ├── handlers/main.yml # Handlers for restarting services
│ ├── templates/
│ │ └── users_registration.j2 # Template for user registration file
│ └── vars/main.yml # Variables (users and passwords)