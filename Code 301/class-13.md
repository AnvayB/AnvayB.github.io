#### In your own words, describe what each group of status code represents:
    100’s = tell the client that the header part of the req has been recieved 
    200’s = tell the client that its req was accepted
    300’s = tell the client that the resource they are requesting isn't available at the expected location
    400’s = tell the client that an invalid request has been made to the server
    500’s = tell the client that the servers are being overwhelmed or are unreachable due to proxies
#### What is a status code 202?
- asynchronous processing of a request
#### What is a status code 308?
- tell the client to use another URL to access the resource
#### What code would you use if an update didn’t return data to a client?
- Error 204: No Content
#### What code would you use if a resource used to exist but no longer does?
- Error 410: Gone
#### What is the ‘Forbidden’ status code?
- Error 403

---

#### Why do we need to pull our MongoDB database string out of our server and put it into our .env?
- so that the Mongo DB is referenced in our code but isn't accessible by external users
#### What is middleware?
- "software glue"
- provides services to software applications beyond those available from the OS
#### What does app.use(express.json()) do?
#### What does the /:id mean in a route?
- it comes from the database by using a function
#### What is the difference beween PUT and PATCH?
- PUT: request URI to supply a modified version of the requested resource
- PATCH: suuplies a set of instrcutions to modify the resource
#### How do you make a default value in a schema?
- make the mongoose string schema type default as value as blank and make the field optional
#### What does a 500 error status code mean?
- Internal Server Error: missing header field in backend >>> third part server is unreachable
#### What is the difference between a status 200 and a status 201?
- 200: the request was recieved and understood and is being processed
- 201: the request was successful and a resource has been created as a result
