# Class 8 reading

## What does REST stand for?

Representational State Transfer, This is a architectual approach to the layout (design) of web services

## REST APIs are designed around a ____

REST API's are designed around "resources" (resources are any kind of data, object, or service that can be accessed my the client.)

## What is an identifier of a resource? Give an example

An URi (uniform resource identifier) is like a "location" or destination for a specific page or resource (i think)

## What are the most common HTTP verbs?

Most common HTTP verbs are:

- GET
- POST
- PUT
- PATCH
- DELETE

## What should the URIs be based on?

a JSON exchange formate

## Give an example of a good URI

``http://mywebsite.com/order/1``

## What does it mean to have a ‘chatty’ web API? Is this a ## good or a bad thing?

This is when there are too any requets on a server, this can cause a problem. This happens when there is a large number of small resources. So this is a bad thing. You need to strike the balance. not a large order of small resources or evem a large order with unneeded resources.

## What status code does a successful GET request return?

200

## What status code does an unsuccessful GET request return?

This gets a representation of the resource at the specific URI. The body contains the details of the request resource.

## What status code does a successful POST request return?

This creates or replaces the resource at the specified URI. The body displays the specified resource to be created or updated.

## What status code does a successful DELETE request return?

This removes the resource of the specified URI.

### Defintions

Hypermedia : lets you build services that decouple client and server to a large extent and let them evolve indepently (from spring.io)

## General notes

 Focus on the business. Certain business might be based around customers and orders. sending POST requests should use a noun which would show if the request went through successfully. as apposed to verbs (the operations on the resource).

 `` https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid``

It is good naming convention to use plural nouns that reference a collection.


### Things i want to know more about

So i kind of understand what this applies to but there is alot of abstractions there, so maybe i need to take a deeper dive to get a clearer picture of everything.