TUTO FOR THIS SITE: https://realpython.com/python-django-blog/#the-postlist-component

A Django Blog Admin, a GraphQL API, and a Vue Front End

saving project on github:
    

run both servers 

>>>>>    backend [PYTHON]

admin, GraphQL

python3 -m venv my_env
source my_env/Scripts/activate   //windows
             /bin/              //unix

python3 -m pip install -r requirements.txt   

//if none exist
python3 manage.py createsuperuser --email admin@example.com --username admin  //if db not present 
python3 migrate                //creates db with default fields like admin and others...  the superuser is saved in here 

python3 manage.py runserver   //to run localhost:8000 backend





>>>>>      in between GraphQL [JSON]

GraphQL API is the alternative to REST API
it generates json 
frontend communicates threw this to fetch data form the backend 

>>>>>    frontend [JS]

can run without django backend running but the db wont be loaded 

npx @vue/cli create frontend --default   //1st installation 
npm -i //just node_modules   when changing os, reinstall 

npm run serve    // to run localhost:8080 frontend 

