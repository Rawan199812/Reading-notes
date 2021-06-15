***Django Custom User***
**There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser.**

***Superuser***
**It's helpful to create a superuser that we can use to log in to the admin and test out log in/log out. On the command line type the following command and go through the prompts.**

- **DjangoX, which is an open-source Django starter framework that includes a custom user model, email/password by default instead of username/email/password, social authentication, and more.**

**Using a custom user model when starting a project**

- If you’re starting a new project, it’s highly recommended to set up a custom user model, even if the default User model is sufficient for you. This model behaves identically to the default user model, but you’ll be able to customize it in the future if the need arises:

from django.contrib.auth.models import AbstractUser
class User(AbstractUser):
    pass

- Reusable apps shouldn’t implement a custom user model. A project may use many apps, and two reusable apps that implemented a custom user model couldn’t be used together. 

**Custom users and the built-in auth forms**

- Django’s built-in forms and views make certain assumptions about the user model that they are working with.


- AuthenticationForm: Uses the username field specified by USERNAME_FIELD.
- SetPasswordForm
- PasswordChangeForm
- AdminPasswordChangeForm

**Custom users and permissions**

***To make it easy to include Django’s permission framework into your own user class, Django provides PermissionsMixin. This is an abstract model you can include in the class hierarchy for your user model, giving you all the methods and database fields necessary to support Django’s permission model.***