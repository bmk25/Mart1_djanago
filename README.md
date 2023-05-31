# stockproj

IMPLEMENTATION DOCUMENTATION
Hardware Requirements:
              1.	Processor: i3, i5, i7 processor
              2.	RAM: 4GB+
              3.	Hard Disk: 20GB+
Software Requirements:
              1.	Operating System : Windows 8 and above 
              2.	Frontend Technology : Html, CSS, Bootstrap, Java Script
              3.	Backend Technology : Python(https://www.python.org/downloads/)
              4.	Framework : Django
              5.	Database : Mysql(https://www.mysql.com/downloads/)
              6.	IDE : VS Code(https://code.visualstudio.com/download)
Steps of implementation:
1.	Modules should be installed in python:
    open the terminal and install these modules
              >pip install mysql
              >pip install mysql.connector 
              >pip install django 
_________________________________________________________________________________________________________________________________________________________________________
2.	Download the SatelliteCohort_Project_1.zip file.
_________________________________________________________________________________________________________________________________________________________________________
3.	Unzip the file in the desired location and Open stockproj folder with the VS Code in the SatelliteCohort_Project_1  folder.
              --> Path for the stockproj folder should be displayed like this 
                  >stockproj/
                            >stockapp
                            >stockproj
                            >templates
                            >manage.py
_________________________________________________________________________________________________________________________________________________________________________
4.  open the Mysql Command line Client and create a database with the given syntax.
               > CREATE DATABASE supermarketdb;
_________________________________________________________________________________________________________________________________________________________________________
5.  Open settings.py file in the stocproj folder and enter your database credentials in DATABASE block like shown below.
   ..............................................................................................................................................................
              --> Path for the setting.py                      
                  >stockproj                                             
                            >stockapp                       
                            >stockproj/                      
                                       asgi.py                                                                 
                                       settings.py                                                              
                                       urls.py                                                                
                                       wsgi.py  
                            >templates
                            >manage.py                                                                         
    ..............................................................................................................................................................           
               --> In the setting.py file modify some changes in the database block   
                          1.Change the password with your MySQL database password
                                   DATABASES = {
                                        'default': {
                                            'ENGINE': 'django.db.backends.mysql',
                                            'NAME': 'supermarketdb',  # Database name
                                            'USER': 'root',
                                            'PASSWORD': 'kiran01',
                                            'HOST': 'localhost',   # Or an IP Address that your DB is hosted on
                                            'PORT': '3306',
                                        }
                                    }
_________________________________________________________________________________________________________________________________________________________________________   
6.   Open the terminal and run the following commands
              1. syntax :> python manage.py makemigrations
                           •	 We run the make migrations command in terminal then django will go to models.py file and check for latest modifications.
                           •	 If any migrations are in ORM language then it will be converted into SQL language

              2. syntax :> python manage.py migrate
                           •	It will create a new python file in migrations folder and save the SQL code.
                           •	If any python file available in models.py then it will take sql code from that file and execute the database, so it will create table as per                                  django model.
 _________________________________________________________________________________________________________________________________________________________________________
 7.   In the terminal Create users by using this command(VScode):
              -->syntax :> python manage.py createsuperuser
              -->Path shown below is only example  
                 1. Create admin user-(for the manager)
                          C:\Users\k.k\Documents\SatelliteCohort_Project_1\stockproj> python manage.py createsuperuser 
                                  Username:       admin 
                                  Email address:  (skip the email)
                                  Password:       (give password) 
                 2. Create staff user-(for the staff users)
                          C:\Users\k.k\Documents\SatelliteCohort_Project_1\stockproj> python manage.py createsuperuser
                                  Username:       (you can give your own name) 
                                  Email address:  (skip the email)
                                  Password:       (give password)
  _________________________________________________________________________________________________________________________________________________________________________
   8.   Now enter the below command for runnig the project with localserver
                --> syntax : python manage.py runserver
                    -->after this it shown like this
                        system check identified 1 issue (0 silenced).
                        May 31, 2023 - 15:59:31
                        Django version 4.1.7, using settings 'stockproj.settings'
                        Starting development server at http://127.0.0.1:8000/
                        Quit the server with CTRL-BREAK.
                    --> click the link you will redirect to the browser
    NOTE: Watch the Satelite_Mart_Demo_video in the SatelliteCohort_Project_1
                 
 
                         
                                               
                      
                         
   
                                            
             
              



