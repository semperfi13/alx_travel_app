# ALX Travel App

A Django-based travel listing platform built with industry-standard best practices for scalable backend development.

## Project Overview

The **alx-travel-app** is a real-world Django application that serves as the foundation for a travel listing platform. This project demonstrates professional Django development practices including modular configurations, database integration, API documentation, and collaborative development workflows.

## Features

- **Django REST Framework** for robust API development
- **MySQL** database integration with secure connection handling
- **Swagger API Documentation** via drf-yasg
- **CORS Headers** configuration for cross-origin requests
- **Environment Variable Management** using django-environ
- **Celery & RabbitMQ** integration for background task processing
- **Modular Project Structure** for maintainability and scalability

## Tech Stack

- **Backend**: Django 4.x, Django REST Framework
- **Database**: MySQL
- **Documentation**: Swagger (drf-yasg)
- **Task Queue**: Celery with RabbitMQ
- **Environment Management**: django-environ

## Quick Start

### Prerequisites

- Python 3.8+
- MySQL 8.0+
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/alx-travel-app.git
   cd alx-travel-app
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Environment setup**
   ```bash
   cp .env.example .env
   # Update .env with your database credentials
   ```

5. **Database setup**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Run the development server**
   ```bash
   python manage.py runserver
   ```

## Project Structure

```
alx-travel-app/
├── alx_travel_app/          # Main project directory
│   ├── __init__.py
│   ├── settings.py          # Django settings with environment variables
│   ├── urls.py              # URL configuration
│   └── wsgi.py
├── listings/                # Core app for travel listings
│   ├── migrations/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   └── urls.py
├── requirements.txt         # Project dependencies
├── .env.example            # Environment variables template
├── .gitignore              # Git ignore file
└── manage.py               # Django management script
```

## API Documentation

Once the server is running, access the Swagger API documentation at:
- **Swagger UI**: `http://localhost:8000/swagger/`
- **ReDoc**: `http://localhost:8000/redoc/`

## Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
SECRET_KEY=your-secret-key-here
DEBUG=True
DATABASE_NAME=alx_travel_db
DATABASE_USER=your-mysql-username
DATABASE_PASSWORD=your-mysql-password
DATABASE_HOST=localhost
DATABASE_PORT=3306
```

## Key Dependencies

- `django`: Core Django framework
- `djangorestframework`: REST API development
- `django-cors-headers`: CORS configuration
- `drf-yasg`: Swagger API documentation
- `django-environ`: Environment variable management
- `mysqlclient`: MySQL database connector
- `celery`: Background task processing
- `rabbitmq`: Message broker for Celery

## Development Workflow

1. **Create feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make changes and commit**
   ```bash
   git add .
   git commit -m "Add your feature description"
   ```

3. **Push to GitHub**
   ```bash
   git push origin feature/your-feature-name
   ```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

This project is developed as part of the ALX Software Engineering Program.

## Support

For questions or issues, please create an issue in the GitHub repository or contact the development team.

---

**Built with ❤️ for ALX Software Engineering Program**