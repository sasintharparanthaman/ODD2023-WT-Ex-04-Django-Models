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

![Screenshot 2023-11-24 103801](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/80af8d59-3c97-4a91-93f9-159cd5893de5)


# step 4: Run the program using the command

Python manage.py runserver 8000

In the admin/ page you can view the models created

And  in the user_profile template page you can see the profile page of the user.

# OUTPUT:
![Screenshot 2023-11-24 101203](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/5f3515b9-a380-4e42-9e93-4320ceeae1dc)
![Screenshot 2023-11-24 105630](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/4cd90ecd-8e02-4875-ac57-8e7db782be82)

# Result:
The djando models created successful.


