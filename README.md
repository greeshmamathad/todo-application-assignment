## Introduction

This is a simple Todo application built off Django (backend - API CRUD operations) and React for frontend.

## Requirements
* Python3
* Pipenv

## Components used:
1. Django - for the backend. This is because it's a very well known, widely used and stable framework across web developers. Very small learning curve for learning, understanding and writing the code.
  An REST API could be written in as less as 10 minutes with right knowledge.
  Used the following components/libraries:
    - django - parent python package that houses all the needed libraries
    - djangorestframework - Needed to work with REST APIs (CRUD opertaions)
    - django-cors-headers
2. React - This has been a very popular option recelty among Frontend developers. I used this for the project because I already have the hands on experience with it in my previous job. 


## Backend data store:
1. Django framework offers database service option out of the box. For this particular project, sqlite database is used which is a type of SQL/structured database. This is used over other database option like postgres because it's very light weight and persists data smoothly even when the application server crashes.
2. A database migration defines the structure of the database table in which the data is stored. Here, it is: "backend/todo/migrations" which defines 4 simple fields to store the dats viz.: 'id', 'title', 'description' and 'completed'

## Deployment Architecture:
1. I don't necessarily have experience with platforms like Heroku, Netlify but I am aware of how things work under the hood and the purpose of deploying on such platforms.

## Roadblocks experienced:
1. My Django experience was pretty minimal until I started working on this project/assignment. I had to learn the Django from scratch and do it myself. Ofcourse, the Django community is pretty solid and provides all answers online. 
2. I could not understand how "serializers" work in Django. But this is not all that bad. I needed serializer to offload the data structuring in API response to Django. 

## GitHub Links
Backend and Frontend codes can be found here: 
1. Backend: 
2. Frontend: 

## URL of Deployments:
To launch the project, follow the below simple instructions:
1. Clone the project to your machine ```[git clone https://github.com/greeshmamathad/todo-application-assignment]```
2. Navigate into the directory ```[cd django-todo-react]```
3. Source the virtual environment ```[pipenv shell]```
4. Navigate to `backend` directory and Install the dependencies 
   ```
   cd backend
   pip install django djangorestframework django-cors-headers
   ```
5. Run the backend django appliction:
   ```python manage.py runserver```
6. Open a new terminal and navigate to the frontend directory ```[cd frontend]```
7. Run the frontend react app ```yarn start```
