web: postgres createuser -P -s -e stegolica-user
web: cd wsgi
web: virtualenv venv
web: source venv/bin/activate
web: postgres createdb -O stegolica-user stegolica
web: cd stegolica
web: cp dev-settings.py settings.py
web: python mange.py migrate
web: python manage.py runserver
