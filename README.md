# NOVA Campus — Branded Student Web Portal

A responsive Django website for the Week 14 Python Programming 2 / Django Templates laboratory activity.

## Features
- Home page with portal introduction and three student-portal features
- About page with portal purpose and accessibility information
- Shared header, navigation, and footer using Django template inheritance
- Reusable feature-card template using `{% include %}`
- Django URL names and template tags (`{% url %}`, `{% static %}`, `{% block %}`)
- Responsive external CSS, custom NOVA CAMPUS logo, keyboard-friendly navigation, and readable contrast

## Requirements
- Python 3.10 or newer
- pip

## Run the project

Open a terminal in the folder containing `manage.py`.

### 1. Create and activate a virtual environment

**Windows (PowerShell):**
```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2. Install Django
```bash
python -m pip install -r requirements.txt
```

### 3. Apply migrations and start the server
```bash
python manage.py migrate
python manage.py runserver
```

### 4. Open the website
Visit http://127.0.0.1:8000/ for Home and http://127.0.0.1:8000/about/ for About.

## Project structure
```text
nova_campus_portal/
├── campus_portal/       # Django project configuration
├── portal/              # Home and About app
├── templates/portal/    # Django HTML templates
├── static/css/          # External stylesheet
├── static/images/       # Custom portal logo
├── manage.py
└── requirements.txt
```

## Customization
Change the portal text in `templates/portal/home.html` and `templates/portal/about.html`.
Update colors and layout in `static/css/style.css`.
The NOVA CAMPUS logo is stored at `static/images/nova-campus-logo.png`.

This project is an original student-work starter implementation based on the supplied Week 14 activity. The logo artwork is custom-generated for this project; no image can be guaranteed impossible to copy.
