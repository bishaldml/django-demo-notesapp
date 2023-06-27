# Simple Notes App
Deploying this simple noteapp built with React and Django in Nginx server.

## Requirements
1. Python 
2. Node.js
3. React

## Installation
1. Clone the repository
```
https://github.com/bishaldml/django-demo-notesapp.git
```
2. Create a virtual environment and activate it
```
virtualenv venv
venv/bin/activate
```
3. Install the requirements
```
pip install -r requirements.txt
```
4. Run the server
```
python manage.py runserver
```

## Frontend - React
5. Open another terminal and navigate to the mynotes directory
```
cd mynotes
```
6. Install the dependencies
```
npm install
```
7. Run the app
```
npm start
```

## Deployment in Nginx
8. Install nginx
```
sudo apt-get update

sudo apt install nginx -y

sudo systemctl restart nginx

sudo systemctl status nginx
```
9. Install docker
```
sudo apt install docker.io
sudo usermod -aG docker $USER
```
10. Build the app
```
docker build -t notes-app
```
11. Run the app / to build container
```
docker run -d -p 8000:8000 notes-app
```
