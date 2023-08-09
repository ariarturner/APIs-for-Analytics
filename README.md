# What is an API  

API stands for Application Programming Interface. They allow computer programs to communicate with each other. While often described as a "handshake", there is another analogy that I think explains it a bit better.  

## Restaurant Analogy  

Let's say you want to eat a croissant.  
You could go to the store and buy all the ingredients and then go home and bake it yourself. There's a lot of work that goes into that and you might not have the technical expertise to do it well (or even at all). Or if you want to eat something more exotic, you might not have the ability to even source the ingredients.  
Instead you might opt to go to a restaurant. The restaurant has a menu with all of the items they serve, and they even categorize it for you so it's easier to find what you're searching for. The restaurant takes care of the sourcing of ingredients and technical labor and expertise. All you need to do is place an order. You don't need to know what ingredients are in it; you don't need to know how it's made. All you need to know is what you want.  
An API is like a restaurant. You *(the client)* put in an order *(the request)* to the waiter *(the API)*. The waiter *(the API)* communicates this order to the kitchen *(the server)*. The kitchen *(the server)* prepares the order *(the request)*, taking care of all the backend processes. The waiter *(the API)* then brings the dish *(the response)* to you *(the client)*.  

### TLDR: Restaurant Analogy  

You *(client)* place an order with the waiter *(API)* at a restaurant. The kitchen *(server)* prepares the order *(request)* and then the waiter *(API)* brings you *(client)* the dish *(response)*.  

## Helpful Tools  

[Postman](https://web.postman.co) may be helpful to get comfortable using APIs and understanding the data that is available.  

# Requests and Responses  

You (the client, which is really your browser) make a request to the server, and the server sends back a response.  

## Request Types  

### GET  

Get data sent to you from the server  

### POST  

Add data to the server  

### PUT  

Update data on the server  

### DELETE  

Delete data from the server  

## Response Types  

### XML  

Used to be most popular, but not used as much anymore  

### JSON  

JavaScript Object Notation  
Current popular format. Returns response as a JavaScript object, which makes it easy to work with in your JavaScript web applications. JSONs are made up of key:value pairs  

## JSON

### JSON Syntax  

Keys are in `""` and are separated from their associated value by a `:`. Key:value pairs are separated by a `,`. The whole set of key:value pairs is enclosed by `{}`. The syntax of values depends on their data type (examples below: `string`, `number`, `boolean`, `null`, `array`, `object`).  
```
{
"key1": "String value",
"key2": 123,
"key3": true,
"key4": null,
"key5": ["item1", "item2", "item3"],
"key6": {"nestedkey1":"String value", "nestedkey2":123}
}
```

### Objects & Dot Notation  

Objects can have properties and methods. Properties are attributes of the object. Methods are actions (functions) that can be applied to the object. Objects and methods use dot notation.  
```
object.method()
object.property
```

### Helpful Methods  

`parse()` transforms a readable string (xml format) into JSON.  
`json()` transforms a response into JSON.  

# API Documentation

## Description

Type of data is available  

## Requirements

Requirements for using API (cost, key, etc.)

## Examples

Examples of how to make requests and reponses returned  

## Endpoints & Parameters

Endpoints are the different places you can connect to the API (URLs). Going back to the restaurant analogy, these are like the categories on the menu.  
```
domain.com/api/endpoint
```
At the end of each URL, parameters can be specified to filter and/or organize the response returned. Usually parameters are denoted by a `?` in front of it, but can also be denoted by a `/`. Multiple parameters are speparated by `&`.  
```
domain.com/api/endpoint?parameter=value
domain.com/api/endpoint?parameter1=value1&parameter2=value2
```
