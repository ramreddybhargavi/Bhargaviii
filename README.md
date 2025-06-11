# Django Internship Project

A production-ready Django project demonstrating backend skills with DRF, Celery, and Telegram integration.

Features:
- JWT-authenticated APIs
- Celery background tasks with Redis
- Telegram bot integration
- Production-ready configuration

Setup:

1. Clone repo:
```bash
git clone https://github.com/yourusername/django-internship-project.git
cd django-internship-project

2. Create virtual environment:
python -m venv venv
source venv/bin/activate

3. Install dependencies:
pip install -r requirements.txt

4.Configure environment:
cp .env.example .env
# Edit .env with your credentials

5.Run migrations:
python manage.py migrate

Running Locally:
Start Django server:
python manage.py runserver

Start Celery worker:
celery -A config worker -l info

Start Telegram bot:
python manage.py runbot
