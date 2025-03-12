# Entities

This folder contains the entity definitions for the project.

# User Entity

## Overview

The User entity represents registered users in the system. It contains essential information for authentication, authorization, and user management.

## Attributes

| Attribute          | Type         | Required | Unique | Description                             |
|--------------------|--------------|----------|--------|-----------------------------------------|
| id                 | UUID         | Yes      | Yes    | Primary identifier for the user         |
| username           | String(50)   | Yes      | Yes    | User's chosen username for login        |
| email              | String(255)  | Yes      | Yes    | User's email address                    |
| password_hash      | String(255)  | Yes      | No     | Hashed password (using bcrypt)          |
| is_active          | Boolean      | Yes      | No     | Whether the user account is active      |
| is_admin           | Boolean      | Yes      | No     | Whether the user has admin privileges   |
| email_verified     | Boolean      | Yes      | No     | Whether the email has been verified     |
| first_name         | String(100)  | No       | No     | User's first name                       |
| last_name          | String(100)  | No       | No     | User's last name                        |
| created_at         | Timestamp    | Yes      | No     | When the user account was created       |
| updated_at         | Timestamp    | Yes      | No     | Last time user data was modified        |
| email_verified_at  | Timestamp    | No       | No     | When the email was verified             |
| last_login_at      | Timestamp    | No       | No     | Last successful login timestamp         |

## Validation Rules

- **username**:
  - Alphanumeric characters only
  - 3-50 characters long
  - Case insensitive uniqueness
  - No spaces allowed

- **email**:
  - Valid email format
  - Case insensitive uniqueness
  - Maximum 255 characters

- **password**:
  - Minimum 8 characters
  - At least one uppercase letter
  - At least one lowercase letter
  - At least one number
  - At least one special character

## Default Values

- `is_active`: true
- `is_admin`: false
- `email_verified`: false
- `created_at`: Current timestamp
- `updated_at`: Current timestamp

## Related Operations

- Password Reset
- Email Verification
- Account Deactivation
- Admin Status Toggle

## Security Considerations

- Passwords are never stored in plain text
- Email verification required for sensitive operations
- Admin status can only be set by existing admins
- Password reset tokens expire after 24 hours
