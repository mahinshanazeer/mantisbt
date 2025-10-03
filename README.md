# MantisBT Self-Hosted Installation

This repository contains a self-hosted instance of **MantisBT (Bug Tracker)** deployed for internal use.  
MantisBT is an open-source issue tracker that provides a web interface to manage bugs, tasks, and feature requests.

---

## Default Credentials

| Username      | Password |
|---------------|----------|
| administrator | root     |

> **Important:** Change the default administrator password immediately after first login to ensure security.

---

## Access

- **Web Interface:** `http://<server-ip-or-domain>/mantisbt`  
- **Database Configuration:** Stored in `<mantisbt-root>/config/config_inc.php`

Example database configuration in `config_inc.php`:

```php
$g_hostname = 'localhost';
$g_db_type = 'mysqli';
$g_database_name = 'mantisbt';
$g_db_username = 'mantisdbuser';
$g_db_password = 'strong_db_password';
$g_crypto_master_salt = 'random-long-string';
