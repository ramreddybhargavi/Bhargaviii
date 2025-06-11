# Django Internship Project

A production-ready Django project demonstrating backend skills with DRF, Celery, and Telegram integration.

Features:
- JWT-authenticated APIs
- Celery background tasks with Redis
- Telegram bot integration
- Production-ready configuration

Setup:

1. Clone repo:
git clone https://github.com/yourusername/django-internship-project.git
cd django-internship-project

2. Create virtual environment:
python -m venv venv
source venv/bin/activate

3. Install dependencies:
pip install -r requirements.txt

4.Configure environment:
cp .env.example .env

5.Run migrations:
python manage.py migrate

Running Locally:
Start Django server:
python manage.py runserver

Start Celery worker:
celery -A config worker -l info

Start Telegram bot:
python manage.py runbot

API Documentation:
Public Endpoint
json
{"status": "ok"}

Protected Endpoint (Requires JWT)
json
{
    "username": "testuser",
    "email": "user@example.com"
}

Environment Variables:
DJANGO_SECRET_KEY - Django secret key
DB_* - Database credentials
REDIS_URL - Celery broker URL
TELEGRAM_BOT_TOKEN - Telegram bot token

Professional Commit History
1. `feat: initial project setup with production-ready config`
2. `feat: add user authentication with JWT support`
3. `feat: implement public/protected API endpoints`
4. `feat: add celery integration with email task`
5. `feat: telegram bot integration with /start command`
6. `docs: complete README with setup instructions`
7. `chore: final code cleanup and validation`

Important Notes
1. Use **python-dotenv** for environment management
2. Implement **JWT authentication** instead of basic tokens
3. Add comprehensive **docstrings** to all functions
4. Include **unit tests** for all core functionality
5. Use **PostgreSQL** in production configuration
6. Implement **rate limiting** on authentication endpoints
7. Add **error handling** to Telegram bot commands

This structure provides:
- Clear separation of concerns
- Production-ready configuration
- Modular design for scalability
- Professional documentation
- Human-readable commit history
- Complete environment configuration
- Detailed setup instructions
