# Symphony App

This Django application includes functionality to save entities from a given URL using Selenium, extract specific data from the page content, and store the data in a MySQL database using Django's ORM.


## Setup
- Clone the repository
```
git clone https://github.com/Shilnasajd/Symphony.git
```
- Create virtual environment

#### Ubuntu
```
sudo apt update
sudo apt install python3-venv
python3 -m venv env
source env/bin/activate
```
#### Windows
```
python -m venv env
env\Scripts\activate
```
-  Install Requirements
```
pip install -r requirements.txt
```
- Install requirements


## Run

- Enter into the project directory

   - Make sure you're in the root directory of your Django 
project where manage.py is located.

#### Ubuntu
```
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver
```
#### Windows
```
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

## Check API's

- Postman collection Link
```
https://drive.google.com/file/d/17jTEB385mZeRMAeAIRBk3FcaHhCCoXrE/view?usp=sharing
```
## MySQL Database setup

- Create a Database
```
CREATE DATABASE demo CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```
- Create a MySQL User
```
CREATE USER 'demo'@'localhost' IDENTIFIED BY 'Demo@123';
```

- Grant Privileges to the User
```
GRANT ALL PRIVILEGES ON demo.* TO 'demo'@'localhost';
```
- Flush Privileges and Exit MySQL
```
FLUSH PRIVILEGES;
EXIT;
```
