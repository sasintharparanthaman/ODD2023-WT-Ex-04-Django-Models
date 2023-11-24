# Ex-04-Django-Models
# AIM:
To develop a admin users with code

# DESIGN STEPS:
# STEP 1:
Create django project and app

# STEP 2:
create a user_profile models in model .py

# STEP 3:
Add the models in the admin interface using the code in admin.py

# STEP 4:
Write the function based view to render the data from the models to the template in view.py

# STEP 5:
Setup the url path for the templates using urls.py

# STEP 6:
In settings.py file add the app created. Now do the migrations process to initiate and save the models

# STEP 7:
Run the program.

# CODE:
1-models.py

from django.db import models

from django.contrib.auth.models import User 

class UserProfile(models.Model):
    user = models.OneToOneField(User, on_delete=models.CASCADE)
    first_name=models.CharField(max_length=100)
    last_name = models.CharField(max_length=100)
    email = models.EmailField()

2-admin.py

from django.contrib import admin

# Register your models here.
from.models import UserProfile

admin.site.register(UserProfile)

from django.shortcuts import render
from django.views import View
from django.contrib.auth.decorators import login_required

3-view.py

# Create your views here.
from .models import UserProfile
@login_required
def user_profile(request):
    user = request .user
    user_profile = UserProfile.objects.get(user=user)
    

    context = {
    'user': user,
    'user_profile': user_profile,
    'firstname': user_profile.first_name,
    'lastname': user_profile.last_name,
    'email' : user_profile.email,
    }

    return render(request , 'modelapp/user_profiles.html',context)

4-url.py

from django.contrib import admin
from django.urls import path 
from myapp import views
from myapp.views import user_profile

urlpatterns = [
    path('admin/', admin.site.urls),
    path('profile/',views.user_profile,name='user_profile'),
]

5-user_profile.html

<!DOCTYPE html>
<html>
<head>
    <title>User Profile</title>
</head>
<body>
    <h1>User Profile</h1>
    <p><strong>Username:</strong>{{ user.username }}</p>
    <p><strong>First Name:</strong>{{ firstname }}</p>
    <p><strong>Last Name:</strong>{{ lastnam e}}</p>
    <p><strong>Email:</strong>{{ user.email }}</p>
    <p><strong>Coustom Profile Data:</strong>{{ user_profile.custom_field}}</p>
    
</body>
</html>

# OUTPUT:
![Screenshot 2023-11-24 101203](https://github.com/sasintharparanthaman/ODD2023-WT-Ex-04-Django-Models/assets/145743219/5f3515b9-a380-4e42-9e93-4320ceeae1dc)

# Result:
The djando models created successful.


