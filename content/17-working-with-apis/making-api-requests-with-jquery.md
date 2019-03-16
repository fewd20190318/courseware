+++
date = "2017-01-22T18:04:24-05:00"
title = "Making API Requests with jQuery"
toc = true
next = "/17-working-with-apis/api-example"
prev = "/17-working-with-apis/api-overview"
weight = 9

+++


## What is Ajax?

- AJAX stands for Asynchronous JavaScript And XML

- The meaning: web applications can send or receive data from the server without requesting an entire page - instead, they can just request or send an arbitrary amount of data

- In frontend development, Ajax Often used to make API requests that will fetch data from another service without having to refresh the web page

{{% notice tip %}}
  Click [here](https://developer.mozilla.org/en-US/docs/AJAX/Getting_Started) for more information about AJAX 
{{% /notice %}}


## CORS

- CORS is the policy that defines this, an acronym that stands for "Cross-Origin Resource Sharing"

- You cannot normally make an AJAX request across different domains

- Some domains don't allow you to ping them from other domains and some do

{{% notice tip %}}
  Click [here](https://www.html5rocks.com/en/tutorials/cors/) for more information about CORS 
{{% /notice %}}


## Using $.ajax

- jQuery offers an `.ajax` method that can be used to make API calls


- Example of an AJAX call using jQuery's $.ajax method

```

    $.ajax({
      url: url,
      type: "GET",
      dataType: 'jsonp',
      data: {term: term},
      success: function(data){
        // execute this function if request is successful
        console.log(data);
      },
      error: function() {
        // execute this function if request fails
        alert('error occurred');
      }
    });

```
- $.ajax properties

 - url: address where the request is being sent
 - type: HTTP method that is being used for the request (i.e. GET, POST, PUT, DELETE), most of the time you'll be using GET or POST
 - dataType: type of data you are expecting from the response

 - data: data to be sent to the server, for GET requests, this info will be added to the url value

 - success: function that will be called if request is successfull

 - error: function that will be called if request fails

{{% notice tip %}}
  Click [here](http://api.jquery.com/jquery.ajax/) more information about the $.ajax method 
{{% /notice %}}

