# Student-Council-Voting-Portal
School's student council voting portal which was created by myself and two other classmates in order to replace the previous use of google forms, The portal was hosted on Gunicorn on a Linux server backed up by Nginx (for reverse proxying). The portal was built using a 3 layer architecture which consists of:

1. The front end consisting of HTML, CSS (Classmate 1)
2. The back end developed by python using Flask and SQL Alchemy (Classmate 2)
3. The Database which is made by MySQL (Me)

The user interacts with the web interface built using HTML, CSS, and JavaScript.
Requests are received by Nginx, which forwards them to Gunicorn, the WSGI server hosting the Flask application.
The Flask backend validates requests, performs business logic, and communicates with the MySQL database.
The database stores and retrieves user credentials, election information, and voting records.
Flask processes the returned data and sends the appropriate response back to the user's browser.

:                User
                  │
                  ▼
       HTML/CSS/JavaScript (Frontend)
                  │
        HTTP Request via Nginx
                  │
                  ▼
        Gunicorn (WSGI Server)
                  │
                  ▼
          Flask Application
                  │
                  ▼
             MySQL Database
                  │
                  ▼
          Flask processes data
                  │
                  ▼
       Response sent back to user

Features:
🎨 Easy-to-use responsive UI design
💪 Robust Configuration of Postings and Candidates
🔐 Automated authentication using random unique generated passwords
💉 Preventing SQLi Attacks using SQLAlchemy
👤 Total User Anonymity and Vote Hashing
📊 Live Analytical Dashboard in the form of a Pie Chart

Technologies Used:
Python 
Flask
MySQL
Pandas
Mathplotlib
SQL Alchemy
Linux 
Gunicorn

My contributions:

Desgined and implimented the relational database
Developed Login credential generation scripts
Built the live election Dashboard
Created data processing utilities using Pandas
Assisted in back end SQL Alchemy code and overall Deployment

