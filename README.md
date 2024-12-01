# **Gym Management System**

## **Overview**
The Gym Management System is a web-based application built using Python, Django, and MySQL. It provides gym administrators and members with an intuitive interface for managing memberships, scheduling workouts, and tracking member activity. With an emphasis on performance and scalability, this system ensures efficient data management and a seamless user experience.

---

## **Key Features**

### **User Registration & Authentication**
- Allows gym members to sign up, log in, and manage their profiles securely.

### **Membership Tracking**
- Tracks the status, validity, and details of gym memberships for each member, including renewal reminders.

### **Workout Scheduling**
- Enables gym members to schedule their workout sessions and track the availability of gym trainers and equipment.

### **Activity Log Management**
- Maintains logs of all user activities, including workouts, sessions, and attendance history for both members and trainers.

### **Admin Dashboard**
- A comprehensive admin interface to monitor gym operations, view member statistics, and manage schedules.

### **Database Optimization**
- Uses MySQL to ensure fast queries and smooth performance even with a large number of members and activity logs.

---

## **Tech Stack**
- **Python** – Programming language for backend development.
- **Django** – Framework for building web applications and APIs.
- **MySQL** – Relational database management system for efficient data storage.
- **HTML/CSS** – Frontend markup and styling for responsive design.
- **JavaScript** – For dynamic and interactive elements.
- **GitHub** – Version control and code repository hosting.

---

## **Installation**

### **Prerequisites**
- Python 3.x
- MySQL
- Django
- pip (Python package installer)

---

### **Step 1: Clone the Repository**
Clone the project repository and navigate into the project directory:
git clone https://github.com/your-username/gym-management-system.git  
cd gym-management-system  

---

### **Step 2: Install Dependencies**
Create a virtual environment (recommended) and install the required libraries:
python -m venv venv  
source venv/bin/activate  # On Windows: venv\Scripts\activate  
pip install -r requirements.txt  

---

### **Step 3: Setup MySQL Database**
1. Create a new database in MySQL:
   CREATE DATABASE gym_management;  
2. Configure the database settings in the `settings.py` file of the Django project:
   DATABASES = {  
       'default': {  
           'ENGINE': 'django.db.backends.mysql',  
           'NAME': 'gym_management',  
           'USER': 'your-mysql-username',  
           'PASSWORD': 'your-mysql-password',  
           'HOST': 'localhost',  
           'PORT': '3306',  
       }  
   }  

---

### **Step 4: Run Migrations**
Run the migrations to set up the database schema:  
python manage.py migrate  

---

### **Step 5: Create Superuser (Admin Access)**
Create an admin account to access the admin panel:  
python manage.py createsuperuser  

---

### **Step 6: Start the Development Server**
Start the development server to test the application:  
python manage.py runserver  

Now, access the Gym Management System in your browser at [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

---

## **Usage**

### **Member Features**
- **Registration & Profile Management**: Members can create an account, log in, and manage their personal details.
- **Workout Scheduling**: Members can book workout sessions based on trainer availability and the gym schedule.
- **Track Progress**: Members can track their workout history and progress.

### **Admin Features**
- **User Management**: Admins can view, add, and delete members.
- **Membership Management**: Admins can manage membership validity and renewals.
- **Schedule Management**: Admins can create and adjust workout schedules.
- **Activity Logs**: Admins have access to member activity logs for monitoring.

---

## **Database Design**
The database consists of the following key tables:
- **Users** – Stores user information (members and admins).
- **Memberships** – Tracks the status of gym memberships (active, expired, etc.).
- **Workouts** – Contains information on workout schedules, types, and trainer assignments.
- **Activity Logs** – Stores data regarding member activities in the gym.

---

## **Contributing**
Contributions are welcome! To contribute:

1. Fork this repository.
2. Create a new branch:  
   git checkout -b feature-name  
3. Make your changes and commit them:  
   git commit -am 'Add new feature'  
4. Push to the branch:  
   git push origin feature-name  
5. Open a pull request.

---

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## **Contact**
For any questions or suggestions, feel free to reach out:  

**Email**: prasad88603@gmail.com  
**GitHub**: https://github.com/SvvDurgaprasad

Enjoy managing your gym effortlessly with the Gym Management System! 🎉💪
