# CRUD 

Create, Read, Update, and Delete (CRUD) are the four basic functions that models should be able to do, at most.



1. **In your own words, describe what each group of status code represents:**
        100's = requestis recieved and the server will try to comply with a transmission demand of the client the request
        200's = request is accepted or at least met all validation requirements at the time of sending
        300's = redirection since requested resources are not available at the requested location anymore
        400's = error for invalid requests
        500's = errors for servers, when servers are unreachable 

2. **What is a status code 202?** request is valid but not processed yet

3. **What is a status code 308?** This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

4. **What code would you use if an update didn't return data to a client?** 204 No content

5. **What code would you use if a resource used to exist but no longer does?** 410 Gone

6. **What is the 'Forbidden' status code?** 403 Forbidden


***



1. **Why do we need to pull our MongoDB database string out of our server and put it into our .env?**
to be hidden so no one can change the path 

2. **What is middleware?**
Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.

3. **What does app.use(express.json()) do?**
It parses incoming JSON requests and puts the parsed data in req

4. **What does the /:id mean in a route?**
it's a dynamic route, so req.params.id will be whatever comes after summary/ in that specific request.

5. **What is the difference between PUT and PATCH?**
PUT is a method of modifying resource where the client sends data that updates the entire resource . PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.

6. **How do you make a default value in a schema?**
You can specify a default value for an item using the default keyword. When a data doesn't have a corresponding value, the value of this keyword will be used instead to do the validation checks

7. **What does a 500 error status code mean?**
 means something has gone wrong on the website's server

8. **What is the difference between a status 200 and a status 201?**
The 200 status code means, simply, that the request was received and understood and is being processed
on the otherhand,
A 201 status code indicates that a request was successful and as a result, a resource has been created

***
## Things I want to know more about

how exactly can we manipulate and use data within mongoDB and how servers can be connected with big data.

***
## External resource 

[Status](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

[CRUD](https://www.codecademy.com/article/what-is-crud)





