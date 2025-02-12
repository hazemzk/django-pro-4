# Django REST Framework API

This project is a **REST API** built using **Django REST Framework**, providing a way to create, manage, and enroll in courses.

## **Requirements**

Before running the project, make sure you have the following installed:
- Python 3.8+
- Django 5.1.3
- Django REST Framework
- PostgreSQL or SQLite (for storage)
- `requests` library (for API testing)

## **Installation & Setup**

1. **Clone the repository:**
```bash
 git clone https://github.com/yourusername/your-repo.git
 cd your-repo
```

2. **Create and activate a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On MacOS/Linux
venv\Scripts\activate  # On Windows
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Run migrations and create the database:**
```bash
python manage.py migrate
```

5. **Create a superuser (optional):**
```bash
python manage.py createsuperuser
```

6. **Start the development server:**
```bash
python manage.py runserver
```

Now, you can access the API at **`http://127.0.0.1:8000/api/`**.

---
## **Features**

### **🔹 Chapter 13: Course & Content Management**
- Adding models and data for course management.
- Creating an admin panel for content management.

### **🔹 Chapter 14: Developing a REST API**
- Building an API using Django REST Framework.
- Defining serializers and API endpoints.

### **🔹 Chapter 15: Authentication & Permissions**
- Implementing authentication using Token Authentication and Basic Authentication.
- Creating custom permissions to control data access.

### **🔹 Chapter 16: Consuming APIs & Service Integration**
- Consuming APIs using the `requests` library in Python.
- Integrating APIs with other systems.

---
## **Consuming the API using Python**

You can use the `requests` library to consume the API as follows:
```python
import requests

base_url = 'http://127.0.0.1:8000/api/'
username = 'your_username'
password = 'your_password'

# Retrieve course list
r = requests.get(f'{base_url}courses/', auth=(username, password))
print(r.json())
```

---
## **Contributors**
- **Your Name Here** - Lead Developer

## **Resources**
- [Django REST Framework](https://www.django-rest-framework.org/)
- [Django Documentation](https://docs.djangoproject.com/en/5.1/)

## **License**
This project is open-source under the **MIT License**.

