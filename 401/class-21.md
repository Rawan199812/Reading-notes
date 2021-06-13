## Django Tutorial Part 3: Using models

- The definition of the model is independent of the underlying database — you can choose one of several as part of your project settings.

- Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata. The code fragment below shows a "typical" model, named MyModelName: from django.db import models


Inside the model:
- Fields : A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. 

- Metadata : is to control the default ordering of records returned when you query the model type. You do this by specifying the match order in a list of field names to the ordering attribute

- Methods : Minimally, in every model you should define the standard Python class method str() to return a human-readable string for each object. This string is used to represent individual records in the administration site.

## Django Admin
- Django does a pretty good job of creating a basic admin site using the information from the registered models:
Each model has a list of individual records, identified by the string created with the model's str() method, and linked to detail views/forms for editing. By default, this view has an action menu at the top that you can use to perform bulk delete operations on records.
- The model detail record forms for editing and adding records contain all the fields in the model, laid out vertically in their declaration order.