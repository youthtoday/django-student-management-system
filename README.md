# Django Student Management System (beta)
This is a Simple Student Management System Developed for Educational Purpose using Python (Django).

## Features of this Project

### A. Admin Users Can
1. See Overall Summary Charts of Stuudents Performance, Staffs Perfomrances, Courses, Subjects, Leave, etc.
2. Manage Staffs (Add, Update and Delete)
3. Manage Students (Add, Update and Delete)
4. Manage Course (Add, Update and Delete)
5. Manage Subjects (Add, Update and Delete)
6. Manage Sessions (Add, Update and Delete)
7. View Student Attendance
8. Review and Reply Student/Staff Feedback
9. Review (Approve/Reject) Student/Staff Leave

### B. Staff/Teachers Can
1. See the Overall Summary Charts related to their students, their subjects, leave status, etc.
2. Take/Update Students Attendance
3. Add/Update Result
4. Apply for Leave
5. Send Feedback to HOD

### C. Students Can
1. See the Overall Summary Charts related to their attendance, their subjects, leave status, etc.
2. View Attendance
3. View Result
4. Apply for Leave
5. Send Feedback to HOD

## How to Install and Run this project?

### Pre-Requisites:
1. Install Git Version Control
[ https://git-scm.com/ ]

2. Install Python Latest Version
[ https://www.python.org/downloads/ ]

3. Install Pip (Package Manager)
[ https://pip.pypa.io/en/stable/installing/ ]

*Alternative to Pip is Homebrew*

### Installation
**1. Create a Folder where you want to save the project**

**2. Create a Virtual Environment and Activate**

Install Virtual Environment First
```
$  pip install virtualenv
```

Create Virtual Environment

For Windows
```
$  python -m venv venv
```
For Mac
```
$  python3 -m venv venv
```

Activate Virtual Environment

For Windows
```
$  source venv/scripts/activate
```

For Mac
```
$  source venv/bin/activate
```

**3. Clone this project**
```
$  git clone https://github.com/vijaythapa333/django-student-management-system.git
```

Then, Enter the project
```
$  cd django-student-management-system
```

**4. Install Requirements from 'requirements.txt'**
```python
$  pip install -r requirements.txt
```

If mysqlclient can't be installed, it is because the dependencies of mysql are not installed. Install libmysqlclient-dev first.

On Ubuntu
```shell
sudo apt-get install update
sudo apt-get install upgrade
sudp apt-get install libmysqlclient-dev
pip install mysqlclient
```

**5. Add the hosts**

- Got to settings.py file 
- Then, On allowed hosts, Add [‘*’]. 
```python
ALLOWED_HOSTS = ['*']
```
*No need to change on Mac.*


**6. Change Databases**

- Go to settings.py file
- Then, change the databases settings to yours.

**7. Now Run Server**
Command for AWS EC2:
```
python manage.py runserver <your-private-ip>:8000
```
Public for browser: /<your-public-ip/>:8000

Command for PC:
```python
$ python manage.py runserver
```

Command for Mac:
```python
$ python3 manage.py runserver
```

**7. Login Credentials**

Create Super User (HOD)
```
$  python manage.py createsuperuser
```
Then Add Email, Username and Password

**or Use Default Credentials**

*For HOD /SuperAdmin*
Email: admin@gmail.com
Password: admin

*For Staff*
Email: josephramos@columbia.edu
Password: josephramos

*For Student*
Email: lijiehuang@gmail.com
Password: lijiehuang
