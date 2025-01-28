### Django application for tracking books reading progress
<br/>

Test task for a course [Advanced Django 5](https://stepik.org/course/177355)

Runs on *Python 3.12.2*

Uses Django ver. 5.1.5

Requires Docker compose installed on local machine

All the requirements are listed in [requirements.txt](/app/requirements.txt)

Currently hosted on: [https://blog.django-project.ru/](http://blog.django-project.ru/)
<br/><br/>

**To run locally use following steps:**

**Start containers:** `docker compose -f docker-compose.prod.yml up -d`

**Migrate DB:** `docker compose -f docker-compose.prod.yml exec web python manage.py migrate --no-input`

**Collect static files:** `docker compose -f docker-compose.prod.yml exec web python manage.py collectstatic --no-input`

**Open in browser:** `http://127.0.0.1/`