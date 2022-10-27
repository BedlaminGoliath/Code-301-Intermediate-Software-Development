# Class 12 Reading

## In your own words, describe what each group of status code represents

100’s = Informational status codes; The head part of the request went through and it will try to do what was asked of it.
200’s = These are successful codes. Or atleast they tell the client that the request went through/ or atleast... met all requirements.
300’s = These let the client know that the location they are sending the request is nolonger valid.
400’s = This is an error saying these are "client errors", this could happend because the requests the client sent through are invlade. (time outs, wrong uri's or missing authentication).
500’s = These usually arise because of a server problem, this could be because overhwhelmed servers or the servers are unreachable.

## What is a status code 202?

This is a "accepted" request (often used with asyncronous processing).  This shows that you made a valid request.

## What is a status code 308?

a "permanent redirect" This is when the server tells the client to use another URL to reach the resourcee. Like when we have several different endpoints for a single resource.

## What code would you use if an update didn’t return data to a client?

(update) 204 (not content)-

## What code would you use if a resource used to exist but no longer does?

a 204 (no content)- this reduces traffic and tells the client that the deletion is complete and it returns no response body.

## What is the ‘Forbidden’ status code?

403

### Build REST API

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?

Because this shows our local host data endpoint, which shouldnt be so easy to find.

## What is middleware?

This is code that gets run when the server gets request and before it gets passed to our routes.

## What does app.use(express.json()) do?

this allows our server to use JSON AS A BODY, instead of a GET or a POST.

## What does the /:id mean in a route?

This means that this is a paramter (params). This would give us access to whatever we pass in after the first slash.

## What is the difference between PUT and PATCH?

This is us choosing what we want to update, we can do this with PATCH. With PUT we would update EVERYTHING.

## How do you make a default value in a schema?

By using the "default" keyword.

## What does a 500 error status code mean?

This means that there is an error on our server.

## What is the difference between a status 200 and a status 201?

201-successful created object when 200 is just a successful. When using a POST route it is good practice to send a 201 (because you created something).

## things I want to know more about

what does it mean when they say "we don’t create endpoint accessible resource when creating an access token..." ?

## overall notes

A status code is a number higher than 100 and smaller than 600. First digit defines the class of the status.
code is for "progromatic recog." and the phrase is for the human to see what is happening.

create action is uually done via the HTTPs POST method.

200-ok

201-created: this is good to signal the back-end resource with the `location` header that would define the URL for the newly created resource.

202 - see above.
