# hoang-ha-mobile


## Group Project 

### create enviroment env for project
py -m pip install venv venv
### run enviroment
./venv/Scripts/Activate
### after That run command line
pip install -r requirements.txt

### add file .env into project hoang_ha_mobile, ex: hoang_ha_mobile/.env
### use to by----- from dotenv import load_dotenv
### load_dotenv()  # take environment variables from .env.
### file .env:
        DB_USER=postgres
        DB_PASSWORD=root
        DB_PORT=5432
        DB_HOST=localhost
### Run Docker Image for Postgres Database
Run docker file:
docker run --name postgres -e POSTGRES_PASSWORD=root -e POSTGRES_DB=hoanghamobile -p 5432:5432 -d postgres

### Create supper user for login admin portal
Create supperuser:
py manage.py createsuperuser