# authapp

A Django authentication project.

## Setup

Requires Python 3.15 or a compatible version.

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

The development server is available at http://127.0.0.1:8000/.

Set the `DJANGO_SECRET_KEY` environment variable to a securely generated value
outside local development. The fallback key in settings is for local development
only. The local SQLite database is excluded from Git; migrations create it when
you run the setup commands.
