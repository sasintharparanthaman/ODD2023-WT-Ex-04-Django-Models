# Ex-04-Django-Models

# AIM:
To develop a admin users with code

# DESIGN STEPS:
# Step1 :Create django project and app using the following commands:
Django-admin startproject mymodels 
Python manage.py startapp myapp

# Step 2:Create a user_profile models in model.py
![Alt text](<Screenshot 2023-12-03 131943.png>)


Add the models in the admin interface using the code in admin.py
![Alt text](<Screenshot 2023-12-03 132006.png>)

Write the function based view to render the data from the models to the template in view.py
![Alt text](<Screenshot 2023-12-03 132031.png>)

Setup the url path for the templates using urls.py

![Alt text](<Screenshot 2023-12-03 132057.png>)


In settings.py file add the app created.

# Step 3: Now do the migrations process to initiate and save the models
Python mange.py makemigrations Python manage.py migrate Create a template as user_profiles.html

![Alt text](<Screenshot 2023-12-03 132349.png>)

# Step 4: Run the program using the command
Python manage.py runserver 8000

In the admin/ page you can view the models created

And in the user_profile template page you can see the profile page of the user.

# OUTPUT:
![Alt text](<Screenshot 2023-11-24 101203.png>)


![Alt text](<Screenshot 2023-11-24 105630.png>)

# Result:
The djando models created successful.