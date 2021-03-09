<p align="center">
    <a href="https://jagrati.herokuapp.com">
        <img src="static/logo.png" width="20%">
    </a>
</p>

<h1 align="center"> 
    Jagrati - An initiative of IIITians
</h1>

Jagrati is an initiative by the students of **IIITDM Jabalpur** to provide free and quality education to the poor and under-privileged children of villages surrounding our institute. 

Currently, we have adopted 5 villages in the vicinity of our institute, namely, Gadheri, Amanala, Chanditola, Mehgawan and Suarkol where we *donate education* to around 100 children of classes 1 through 10. Apart from providing basic education to the students in regular classes, **we also prepare the students of 4th and 5th grade for the prestigious Navodaya Vidyalaya** and other similar government-funded institutions which provides quality education to students, completely free of cost.

Apart from teaching the children, we do many other activities like **organizing Blood Donation Camps, Tree Plantation Drives, Cloth Donation, Stationery Distribution, Campaigns to spread awareness in villages, etc.**

**Our Achievements:**
- 1 student selected in Jawahar Navodaya Vidyalaya in 2018.
- 1 student selected in Jawahar Navodaya Vidyalaya in 2019.
- 2 students selected in Jawahar Navodaya Vidyalaya in 2020.
- 4 students cleared entrance examination for Eklavya Model Residential School (EMRS) in 2020.
- 4 students cleared entrance examination for Gyanodaya Vidyalaya in 2020.

(Like Navodaya Vidyalaya, both EMRS and Gyanodaya Vidyalaya provide free quality education to students from class 6 to 12).

Currently, we are operating in online mode to prepare students of class 5 for Navodaya Examination, 2021.

## About JagratiWebApp
JagratiWebApp is the **official web application** for managing day-to-day operations at Jagrati, like keeping track of the content being taught in a class and homework being given to the students, taking and keeping record of student and volunteer attendance, keeping record of all the students being taught under the initiative and the volunteers contributing towards the initiative among many things.

The main aim of the application is to simplify the work of volunteers by making all the information readily accessible to them like what was taught in the last class or in the last week and how many student attended those classes so that they can easily decide what should be taught on the present day and update the same in the application. Plus, it also helps in taking the attendance of students with more ease over the conventional method of manually taking note of the names of all the students present.

So, all in all, it is meant to help the volunteers work more effectively and efficiently and make it easy to keep track of daily activities.

## Technology Stack

**Frontend:** HTML, CSS(+ Bootstrap 4), JavaScript  
**Backend:** Python/Django  
**Database:** SQL (SQLite3/MySQL/PostgreSQL)  

And additional requirements are in [**requirements.txt**](https://github.com/garg3133/JagratiWebApp/blob/master/requirements.txt)

## To-Do

### New pages

- [ ] List of all Students
- [ ] List of all Volunteers
- [x] Student Profile
- [x] Volunteer profile
- [ ] Update Student Profile
- [ ] Update Volunteer Profile
- [x] Add new Student
- [ ] Calendar containing class schedule, events and other national/international important dates.
- [ ] Page for Managing Permissions
- [ ] Page for viewing and managing feedbacks
- [ ] Web Team Page

### New Apps

- [ ] Jagrati Inventory
- [ ] Events
- [ ] Meetings
- [ ] Study Material

### New Features

- [ ] Notifications
- [ ] Leaderboard (no. of hours contributed to Jagrati)


## Contributing

### Setting-up the project

<details><summary>Step 1 : Downloading and Installing the Code Editor</summary>
 
 
| **Code Editor** | **Link** 	|
|-	|-	|
| Visual Studio Code 	| [Download it from here](https://code.visualstudio.com/)	|
| Sublime Text 3 	| [Download it from here](https://www.sublimetext.com/3) |
| Atom 	| [Download it from here](https://atom.io/)	|


</details>


---


<details><summary>Step 2 : Installing Python 3.7</summary>
 

* For Windows : Click on [Download Python](https://www.python.org/downloads/release/python-379/) 
   * * Download the Windows x86-64 executable installer for 64-bit version of Windows
   * * Download the Windows x86 executable installer for 32-bit version of Windows.

   * * Make sure to check "Add Python 3.7 to Path" in the setup window of the Installer.


* For Linux(Ubuntu) :
   * * Follow the first mehod of [this article](https://linuxize.com/post/how-to-install-python-3-7-on-ubuntu-18-04/)


Verify the installation from the command prompt / terminal using following command :
```
python3.7 --version
```
And the installed version of python will be printed:
```
Python 3.7.x
```


</details>


---


<details><summary>Step 3 : Installing Git </summary>

Click on [Download Git](https://git-scm.com/downloads)

</details>


---


<details><summary>Step 4 : Fork the Repository </summary>

Click on ![Fork](https://user-images.githubusercontent.com/63921263/110382285-b07bba80-8080-11eb-8407-d354849c1753.png)
to fork [this Repo](https://github.com/garg3133/JagratiWebApp)

</details>


---


  * Download and install Python 3.7
  * Download and install Git.
  * Fork the Repository.
  * Clone the repository to your local machine `$ git clone https://github.com/<your-github-username>/JagratiWebApp.git`
  * Change directory to JagratiWebApp `$ cd JagratiWebApp`
  * Install virtualenv `$ pip3 install virtualenv`
  * Create a virtual environment `$ virtualenv env -p python3.7`  
  * Activate the env: `$ source env/bin/activate` (for linux) `> ./env/Scripts/activate` (for Windows PowerShell)
  * Install the requirements: `$ pip install -r requirements.txt`
  * Create a new file in the root directory of the repository (`JagratiWebApp`) with name `.env` (only `.env` and not `.env.txt`) and add the following content in it:
    ```
    EMAIL_HOST_USER = 'your-email@domain.com'
    EMAIL_HOST_PASSWORD = 'your-password'

    SENDER_EMAIL = 'Jagrati <your-email@domain.com>'
    ADMINS_EMAIL = ['email-address-of-admin@domain.com']

    SOCIAL_AUTH_GOOGLE_OAUTH2_KEY = 'google-oauth2-key'
    SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET = 'google-oauth2-secret'
    ```  
    or, just copy the `.env.save` file from `samples` directory to the root directory (`JagratiWebApp`) and rename it to `.env` (only `.env` and not `.env.txt`)  
  
    where, 
    * `EMAIL_HOST_USER` and `SENDER_EMAIL` is the email address of your Gmail account from which you want to send emails (By default, Django will output email contents in console. To actually send emails to real users, comment line 27 and uncomment line 28 in `Jagrati/settings/development.py`).
    * `EMAIL_HOST_PASSWORD` is the password for that Gmail account.
    * `ADMINS_EMAIL` is a list of email addresses of Admins of the site (who will recieve important updates from the site like when a new user joins in).
    * `SOCIAL_AUTH_GOOGLE_OAUTH2_KEY` and `SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET` are the API keys for login/signup using Google.

    **Note:** All the changes mentioned above in the `.env` template are *optional* and you do not need to change anything if you want all the email contents to be printed in the console itself and you do not wish to use login/signup through Google. The changes in the first 4 lines on `.env` file are required only if you wish to send out real emails to real people and changes in last 2 lines are required only if you wish to use login/signup through Google.
  * Copy `sample-db.sqlite3` from `samples` directory to the root directory (`JagratiWebApp`) and rename it to `db.sqlite3`.
  * Make migrations `$ python manage.py makemigrations`
  * Migrate the changes to the database `$ python manage.py migrate`
  * Create admin `$ python manage.py createsuperuser`
  * Run the server `$ python manage.py runserver`

 ### Setting-up the project in docker

  * Fork the Repository.
  * Clone the repository to your local machine `$ git clone https://github.com/<your-github-username>/JagratiWebApp.git`
  * Change directory to JagratiWebApp `$ cd JagratiWebApp`
  * Copy the `.env.save` file from `samples` directory to the root directory (`JagratiWebApp`) and rename it to `.env` (only `.env` and not `.env.txt`).  
    
    (Read the [above](https://github.com/garg3133/JagratiWebApp#setting-up-the-project) section for details on all the variables used in `.env` file)
   
  * Copy `sample-db.sqlite3` from `samples` directory to the root directory (`JagratiWebApp`) and rename it to `db.sqlite3`.
  * Build the docker file to an image `sudo docker build -t <IMAGE_NAME> .`
  * Run the docker image `sudo docker run -p 8000:8000 <IMAGE_NAME>`
  * The server will start at default port (8000), head over to your web browser to test.


### Contributing Guidelines 
  * Feel free to open an issue to report a bug or request a new feature.
  * Before starting to work on an issue, comment on that issue that you want to work on this and then only start to code.
  * Create a new branch with a related name of the motive i.e. bug/refactor/feature and commit your changes in that branch only.  
  * Send a pull request anytime :)  
  * Join our Discord Community: https://discord.gg/Ek9q45ZjAv

## 💥 How to Contribute ?
- If you wish to contribute kindly check the [CONTRIBUTING.md](https://github.com/garg3133/JagratiWebApp/blob/master/CONTRIBUTING.md)🤝
