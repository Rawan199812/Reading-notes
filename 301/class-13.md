## Update/Delete

***The form-data can be sent as URL variables (with method="get") or as HTTP post transaction (with method="post").***

**The "GET" Method**
- Appends form-data into the URL in name/value pairs.

- The length of a URL is limited.

- Never use GET to send sensitive data.

- Useful for form submissions where a user wants to bookmark the result.

- GET is better for non-secure data, like query strings in Google.

**The "POST" Method**
- Appends form-data inside the body of the HTTP request.

- Has no size limitations.

- Form submissions with POST cannot be bookmarked.
### FORM
***An HTML Form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.***

**Form action attribute**

***The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form.***


***the web uses a client/server architecture that can be summarized as follows. a client sends a request to a server, using the HTTP protocol. The server answers the request using the same protocol.***