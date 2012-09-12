Replace 'proj' with project name

cd into project directory

virtualenv venv --distribute

source venv/bin/activate

pip install -r requirements.txt

run Postgres.app

psql -h localhost
> CREATE DATABASE proj;

Run Server
> python manage.py runserver --settings="proj.settings.dev"

Sync DB
> python manage.py syncdb --settings="proj.settings.dev"

Migrate DB 
> python manage.py migrate --settings="proj.settings.dev"

Run Server
> python manage.py runserver --settings="proj.settings.dev"
