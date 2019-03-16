+++
date = "2017-01-22T18:04:24-05:00"
title = "API Overview"
toc = true
prev = "/17-working-with-apis/json"
next = "/17-working-with-apis/making-api-requests-with-jquery"
weight = 8

+++


## What is an API?

- Stands for "Application Programing Interface"

- A way to exchange data between servers / services (i.e. software to software communication)

- Set of programming instructions and standards for accessing a Web-based software application or Web tool

- For example, Amazon.com released its API so that Web site developers could more easily access Amazon's product information

- In a nutshell, if you want to leverage information from another website or application your first choice should be to use an API (if they offer one)


## API Considerations

- Does the website I need data from even have an API?

- Do I need to authenticate with the remote data source before retrieving the information I need, either as an API consumer or as a user of that service?

- What are the URLs I use to access the data I need? In API terms, these URLs are known as "endpoints" and can usually be found in an API's documentation


## What happens when no API is available?

- If the website you need data from does not have an API, you could resort to data scraping through the use of "spiders" which crawl websites and extracts information

- Many online services consider data scraping to be a violation of their Terms of Service


## API Data Formats

- The "modern standard" for API responses is JSON, or JavaScript Object Notation

- Some APIs are implemented using XML, this includes the API for WordPress, which is implemented using the XML-RPC standard


## Request, Response lifecycle

- When making an API call, you are essentially making an **Request** to a server and then receiving a **Response**

- Most of the time this response will contain data that you will make use of within your application
