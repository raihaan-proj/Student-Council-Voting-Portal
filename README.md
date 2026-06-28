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

```text
                 User
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
* 🎨 Easy-to-use responsive UI design
* 💪 Robust Configuration of Postings and Candidates
* 🔐 Automated authentication using random unique generated passwords
* 💉 Preventing SQLi Attacks using SQLAlchemy
* 👤 Total User Anonymity and Vote Hashing
* 📊 Live Analytical Dashboard in the form of a Pie Chart

Technologies Used:
Python 
Flask
MySQL
Pandas
Matplotlib
SQLAlchemy
Linux 
Gunicorn

 
Team Contributions

* Riyaz (@healthboost213): Flask Backend Development and Linux Deployment
* Raihaan (@raihaan-proj): MySQLDB Architecting and Deployment Work
* Shaarvin (@Shaarvin-67): HTML + CSS Frontend Development

This project was developed collaboratively by a team of three students.

* **Frontend Development (Shaarvin):** Designed and implemented the user interface using HTML, CSS, and JavaScript, creating a responsive and user-friendly voting experience.
* **Backend Development (Riyaz):** Developed the Flask application, implemented the application logic, integrated SQLAlchemy, and managed request handling and authentication.
* **Database & Analytics (Raihaan):** Designed the MySQL relational database schema, developed credential generation scripts, created data processing utilities using Pandas, built the live election analytics dashboard with Matplotlib, and assisted with backend database integration and deployment.

Each team member was responsible for a core component of the system while collaborating closely throughout development, testing, and deployment.



My contributions:

Desgined and implimented the relational database
Developed Login credential generation scripts
Built the live election Dashboard
Created data processing utilities using Pandas
Assisted in back end SQL Alchemy code and overall Deployment

Project Highlights

Successfully deployed for a live student council election.
Replaced the previous Google Forms voting process with a dedicated web application.
Hosted on a Linux server using Nginx and Gunicorn.
Included a live analytics dashboard for monitoring election results.
