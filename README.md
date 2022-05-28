# TIMEIT ATTENDANCE MANAGEMENT

In this project, an attendance management system is developed that uses facial recognition to track employee presence, time-in, and time-out. It includes facial detection and identification, as well as the creation of a web application to support the system's many use cases, such as new employee registration, photo addition to the training dataset, reading attendance records, and so on. This project aims to provide a cost-effective alternative to standard manual attendance methods. It can be utilised in places like corporate offices, schools, and businesses where security is a must.

The goal of this project is to automate the traditional attendance method, which involves manually marking attendance. It also allows an organisation to keep track of in-time, out-time, and presence, absence of employees in a digital format.

## Functionality Supported
**This system mainly works around two types of user**
1. Employee
2. Admin

**Functionalities accessible to admin: <br>**
• Login <br>
• Register new employees to the system <br>
• Add employee photos to the training data set <br>
• Train the model <br>
• View attendance report of all employees. Attendance can be filtered by date or employee. <br>

**Following functionalities can be performed by the employee: <br>**
• Login <br>
• Mark his/her time-in and time-out by scanning their face <br>
• View attendance report of self <br>

## Built Using
- **OpenCV** - Open Source Computer Vision and Machine Learning software library
- **Dlib** - C++ Library containing Machine Learning Algorithms
- **face_recognition** by Adam Geitgey 
- **Django**- Python framework for web development.

### Libraries used for Face Detection
- Dlib's HOG facial detector.
- Dlib's 68 point shape predictor
- face_recognition API by Adam Geitgey

## How To Run ?
- Clone it to your device / Download the zip folder of the project and extract
- Make a virtual environment in the project directory
- Install the dlib library following the instructions from [this](https://learnopencv.com/install-dlib-on-ubuntu/) blog for Ubuntu and [this](https://learnopencv.com/install-dlib-on-windows/) for Windows
- Run **``` pip install -r requirements.txt```** inside the directory
- Run **``` python manage.py createsuperuser ```** and fill the required details to create a superuser
- Run **``` python manage.py migrate ```**
- Run **``` python manage.py runserver ```** and follow the link generated to run the project
 
**To access the admin functionalities: <br>**
After running the project you can access all functionalities meant for employees. To access the admin account:
- Go to the django admin page using [this](http://127.0.0.1:8000/admin/) address and login with your superuser credentials
- Go to the Users model->admin username
- Change the password for the admin and use these new credentials to log into the admin dashboard

## Future Scope
1. For offices which need high security, an intruder alert can be incorporated in the project, so that an alert is given to the security whenever an unknown face is detected by the system.
2. The training time can be reduced by retraining the classifier only for the newly added images.
3. A feature can be added such an employee is automatically notified if his attendance or working hours are less than what is required .

**Thank You**