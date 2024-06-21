- [STATUS CODES](#status-codes)
  - [1. Informational Responses](#1-informational-responses)
  - [2. Successful Responses](#2-successful-responses)
  - [3. Redirectional Messages](#3-redirectional-messages)
  - [4. Client Error Responses](#4-client-error-responses)
  - [5. Server Error Responses](#5-server-error-responses)


# STATUS CODES

These are codes used to show or indicate the success of a HTTP request. They are mainly categorized into five groups as discussed below:

 ## 1. Informational Responses
   They range from `100` to `199`.  
   They are used to indicate that a server is working on the user request.  
   They include:

- **100** - Indicate that the user should continue with the request.
- **101** - Indicate that the server is switching to another protocol as per users request.
- **102** - Indicate that the server is still working on the request and is yet to give a response.
- **103** - Indicate that the user should start preparing resources needed by the page which the response to their request will originate.

## 2. Successful Responses
   They range from `200` to `299`  
   They serve to show that a request was sucessful.  
   They include:

- **200** - This is the basic code that shows a request succededed.
- **201** - This indicate that a request to create a resourse was successful.
- **202** - This indicates that the request was recieved successfully but yet to be acted upon.
- **203** - This indicates that the collected metadata is not available in the server, works as `200`.
- **204** - This shows that the request was successful but there is no content to be returned.
- **205** - This responds to a request to indicate that the user should reset the content.
- **206** - This indicates that the only part of resourse has been requested.
- **207** - This stands for multiple status codes in a situation where the information is from various resources.
- **226** - This indicates that the responce is a representation of an edited version of a `GET` request to a resource.

## 3. Redirectional Messages
   They range from `300` to `399`  
   They are used to indicate that more action is neede from the user for the request to be complete.  
   They include:

- **300** - Indicate that the request has more that one response, therefore the user has to choose.
- **301** - Indicate that the requsted resource has been changed permanently to a new URL which is provided.
- **302** - Indicates that the requested resource has been temporarily changed to a new URL which is provided.
- **303** - Indicate that the user is directing the user to get the requested resource in another URI.
- **304** - Indicate that the user can continue using the response cached version because it has not yet been modified.

## 4. Client Error Responses
   They range from `400` to `499`  
   They are used to indicate that there was an error in the client side of the request.  
   They include:

- **400** - Indicate that the server will not work on the request because there is a client error.
- **401** - Indicates that the user is not authenticated, and cannot get the response till they are authenticated.
- **403** - Indicates that the user does not have rights to access the content requested.
- **404** - Indicates that the server cannot find the requested resource.
- **408** - Indicate that the server would lke to shutdown the connection because it is idle.
- **414** - Indicate that the URI requested is too long for the server to handle.
- **415** - Indicates that the media format of the request is not supported by the server.
- **429** - Indicates that the user has sent too many requested in a given amount of time.

## 5. Server Error Responses
   They range from `500` to `599`  
   They are used to indicate that there was an error on the server while handling the request.  
   They include:

- **500** - Indicates that the server encountered an unexpected error that it can't handle.

- **501** - Indicates that the request method used is not recognized by the server and therefore can't be handled.

- **502** - Indicates that the server got an invalid response while trying to get the response for the request as a gateway.

- **503** - Indicates that the server is currently unable to handle the request due to an overload or maintenance issues.
- **504** - Indicates that the server cannot get the response as gateway in time.
- **505** - Indicates that the HTTP version in the request is not supported.
- **506** - Indicates that the server has an internal configuration error.
- **507** - Indicates that the server has insufficient memory to store the representation of the requested resource.
- **508** - Indicate that the server has detected an infinite loop while processing the request.
- **510** - Indicates that further extensions are required for the server to complete the request.
- **511** - Indicates that the user needs to be authenticated to gain network access.
