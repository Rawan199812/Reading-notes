## Django Tutorial Part 9: Working with forms

**HTML Form**
***A group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server.***
- Forms are a flexible mechanism for collecting user input.
- Forms are a relatively secure way of sharing data with the server.

***The role of the server is first to render the initial form state — either containing blank fields or pre-populated with initial values. After the user presses the submit button, the server will receive the form data with values from the web browser and must validate the information.***

- For forms that use a POST request to submit information to the server, the most common pattern is for the view to test against the POST request type (if request.method == 'POST':) to identify form validation requests and GET (using an else condition) to identify the initial form creation request. I

**Django provides a number of tools and approaches. The most fundamental is the Form class, which simplifies both generation of form HTML and data cleaning/validation.**

- get_object_or_404(): Returns a specified object from a model based on its primary key value, and raises an Http404 exception (not found) if the record does not exist.
- HttpResponseRedirect: This creates a redirect to a specified URL (HTTP status code 302).
- reverse(): This generates a URL from a URL configuration name and a set of arguments. It is the Python equivalent of - the url tag that we've been using in our templates.
- datetime: A Python library for manipulating dates and times.

***Creating and handling forms can be a complicated process! Django makes it much easier by providing programmatic mechanisms to declare, render, and validate forms. Furthermore, Django provides generic form editing views that can do almost all the work to define pages that can create, edit, and delete records associated with a single model instance.***
