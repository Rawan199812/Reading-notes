
## How I explained REST to my brother
How web works
- HTTP protocol written by Roy
- HTTP part specifies what protocol to use
- HTTP is like a GPS coordinate for information and knowledge 


- Whole web is architectural style of REST

REST: defintion of resource Web Page kind of represention of a resource
- URL tells where the concept of the resources are

Most resources have a single representation
- APIs are different version/representations of informations

Also called web services
- URLs tell machine where to get information

Since each language is unique nouns?
## SuperAgent

- progressive ajax API created for flexibility and is compatible with node.js
request

- a request can be made by invoking a method on the request object, then calling .then() or end() or await() to send request
.get('/search')
.then(res => {
    //res.body, res.headers, res.status
})
.catch(err => {
    //err.message, err.response
});
request('GET', '/search').then(success, failure);


- head requests use .query() methods
- post/put requests calls then waits for the response string
