# Profiles REST API

A fully functioning REST API that handles user profile creation and management, built with Python, Django, and Django REST Framework. This project implements token-based authentication, user profile management, and feed API functionality.

## Features

- User Profile:
  - Create, read, update, and delete user profiles
  - Email and name-based user registration
  - Password validation
  - Token-based authentication
- Profile Feed API:
  - Create, update, delete status updates
  - View profile feed items
- Permissions:
  - Manage own profile
  - Update own status feed
  - View other profiles

## Technology Stack

- Python 3.x
- Django 3.x
- Django REST Framework
- SQLite (development)
- Vagrant/VirtualBox (development environment)

## Getting Started

### Prerequisites

- Python 3.x
- Vagrant
- VirtualBox

### Installation

1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/profiles-rest-api.git
cd profiles-rest-api
```

2. Create and start Vagrant environment
```bash
vagrant up
vagrant ssh
```

3. Create and activate virtual environment
```bash
python -m venv ~/env
source ~/env/bin/activate
```

4. Install requirements
```bash
pip install -r requirements.txt
```

5. Run migrations
```bash
python manage.py migrate
```

6. Start development server
```bash
python manage.py runserver 0.0.0.0:8000
```

### API Endpoints

- `/api/profile/`: List all user profiles
- `/api/profile/feed/`: Create and list feed items
- `/api/login/`: Get auth token

## Development

The project uses Vagrant for consistent development environments. To start development:

1. Make changes in your local environment
2. Test changes within Vagrant environment
3. Commit and push changes

## License

This project is licensed under the MIT License

## Acknowledgments

- Based on the course project from London App Developer
- Django REST Framework documentation
```
