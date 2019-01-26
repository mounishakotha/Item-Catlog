# Item-Catlog
It is a part of **Udacity Nanodegree Full Stack Project.**

## Introduction ##
This project is about developing a web application using Flask framework and accessing database using *CRUD* operations and also providing *Authentication* by Google and Facebook API's.

## Technologies Used ##
- Python
- HTML
- CSS
- Flask
- Jinja2
- SQLAchemy
- OAuth
- Google Login

##  Prerequisites ##
* Vagrant
* VirtualBox
* Python

## Installation process ##
*  Download [vagrant](https://www.vagrantup.com/downloads.html) and [virtualbox](https://www.virtualbox.org/wiki/Download_Old_Builds_5_1)
* After installing  vagrant and virtualbox, the process as follows:

#### First Step,
* We need to copy our project folder to the place where vagrant is present
```
	vagrant up
	vagrant ssh
```
#### Second Step,
* After connection established install the softwares need to execute the the project as follows:
```
  	cd vagrant
	sudo apt-get install pyhton3
	sudo apt-get install python-pip
	pip install flask --user
	pip install sqlalchemy --user
  	pip install oauth --user
  	pip install oauth2client --user
  	pip install requests --user
```
* To create google OAuth credentials.The steps are as follows:

1) Go to your app's page in the [Google APIs Console](https://console.developers.google.com/apis)
2) Choose Credentials from the menu on the left.
3) Create an OAuth Client ID.
4) This will require you to configure the consent screen, with the same choices as in the video.
5) When you're presented with a list of application types, choose Web application.
6) You can then set the authorized JavaScript origins, with the same settings as in the video.
7) You will then be able to get the client ID and client secret.

You can also download the client secret as a JSON data file once you have created it.
  
#### Third Step,
```
	cd (project folder nmae)
```

#### Fourth Step,
* For first time run database file and data file
```
Run database file 
		python database.py
Run database with some data file
		python cheeseitems.py
Run application file
		python projectflask.py
```
Open browser and vist  [http://localhost:8000](http://localhost:8000)

## JSON endpoints
* In my project the main JSON-endpoints are as follows:
#### Display all cheese-country, cheese-items
```
	/cheese
	/cheese/<int:cheese_id>/
```
####  Add cheese-country, cheese-items
```
	/cheese/addcheese
	/cheese/<int:cheese_id>/new'
```

####  Edit cheese-country, cheese-items
```
	/cheese/<int:cheese_id>/edit
	/cheese/<int:cheese_id>/<int:item_id>/edit'
```
####  Delete cheese-country, cheese-items
```
	/cheese/<int:cheese_id>/delete
	/cheese/<int:cheese_id>/<int:item_id>/delete'
```
#### To see data in a JSON format
```
	/cheese/<int:cheese_id>/JSON
```
## Output Screenshots
* Here some screenshots how my project will appear
	* Screenshot of JSON file
	

