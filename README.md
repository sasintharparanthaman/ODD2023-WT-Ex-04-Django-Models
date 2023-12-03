# Ex-04-Django-Models
# AIM:
To develop a admin users with code

# DESIGN STEPS:

# Step1 : Create django project and app using the following commands:

Django-admin startproject mymodels
Python manage.py startapp myapp

# Step 2: create a user_profile models in model.py

![Screenshot 2023-11-24 103653](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/441fc9fe-2142-4b3c-a9ee-662b6485dd03)


Add the models in the admin interface using the code in admin.py

![Screenshot 2023-11-24 103707](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/dc8d97dd-820a-4067-9666-a16f56e3bd6f)



Write the function based view to render the data from the models to the template in view.py
![Screenshot 2023-11-24 103728](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/341c3119-6283-4528-9ab7-f5886609f0e6)


Setup the url path for the templates using urls.py

![Screenshot 2023-11-24 103748](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/d3c304d0-5ad2-4d35-a4ed-a5d22e0a8ba2)


In settings.py file add the app created.

# Step 3: Now do the migrations process to initiate and save the models

Python mange.py makemigrations
Python manage.py migrate
Create a template as user_profiles.html
![Screenshot 2023-12-03 132349](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/4eb237bd-a29f-4e32-8c1e-47824dc6da32)



# step 4: Run the program using the command

Python manage.py runserver 8000

In the admin/ page you can view the models created

And  in the user_profile template page you can see the profile page of the user.

# OUTPUT:
![Screenshot 2023-11-24 105852](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/258beb93-46e2-43f0-a5a9-77ffe03c5fbf)

![Screenshot 2023-11-24 105630](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/4cd90ecd-8e02-4875-ac57-8e7db782be82)

# Result:
The djando models created successful.



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
![Screenshot 2023-12-03 132349](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/dcd5d1e4-8c9d-439c-9d1e-9f70f4202ee6)



# Step 4: Run the program using the command
Python manage.py runserver 8000

In the admin/ page you can view the models created

And in the user_profile template page you can see the profile page of the user.

# OUTPUT:
![Screenshot 2023-11-24 101203](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/a1412b5b-2120-4300-992f-5d333df229c6)
![Screenshot 2023-11-24 105630](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/fd4ce2f2-f848-45b6-abb3-285340a6ef6e)


# Result:
The djando models created successful.
