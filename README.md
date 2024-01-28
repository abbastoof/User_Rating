**USER Rating API**
---------
Goal 
- In this exercise, I used authentication and validation mechanisms inside DRF.
- The goal of this API is to recieve user review for menu items of LittleLemon restaurant.

Objectives

- Add form validators to form data        

- Perform token and session authentication while using a DRF form      

- Use the Djoser and authtoken packages for default routes

- Use the Django admin panel for creating new users and tokens

Installation
------------

**Note: Pipenv requires Python 3.7 or higher. Please ensure you have Python 3.9 installed to view the results of this project.**

We recommend installing Pipenv using `pip`. Use the following command to install Pipenv:

```bash
pip install --user pipenv
```

After installing Pipenv, navigate to your project directory and activate the Pipenv shell. Then, install the necessary packages:

```bash
pipenv install django
pipenv install djangorestframework
pipenv install djoser
```

Next, migrate your database:

```bash
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver
```

Finally, open the API request client, Insomnia, and perform the following actions:

* Create a POST request to the URL: http://127.0.0.1:8000/api/ratings
* You need to create some users and add a user token in the Insomnia app API request. Create a Form URL Encoded. Add `menuitem_id` as a key and a small integer as a value, add `rating` as a key and a value between 0-5.
