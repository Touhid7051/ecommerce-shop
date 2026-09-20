# Full-Stack Shop API

Django REST API for products, categories, orders,
and dashboard counts.

## Features

- Product and category APIs
- Search, filtering, sorting, and pagination
- Order creation and Django admin
- Cloudinary product images on Render

## Technology

- Django and Django REST Framework
- PostgreSQL, Cloudinary, and Render

## Local Setup

~~~bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
~~~

Windows activation:

~~~powershell
venv\Scripts\Activate.ps1
~~~

## Environment Variables

~~~text
SECRET_KEY=your_local_secret
DEBUG=True
DATABASE_URL=your_database_url
ALLOWED_HOSTS=127.0.0.1,localhost
CORS_ALLOWED_ORIGINS=http://localhost:3000
~~~

Cloudinary variables are private Render settings.

## Main Endpoints

- /api/v1/categories/
- /api/v1/products/
- /api/v1/orders/
- /api/v1/dashboard/counts/
- /admin/

## Deployment

API: https://YOUR_API.onrender.com