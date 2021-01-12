# HTTP

## Overview

- **HTTP** - HyperText Transfer Protocol
- Set of rules for querying the web
- Client <-HTTP request/response-> Server
- - Client makes requests that contains methods, headers, body
- - Server receives request and sends a response that contains status, headers, body

## Methods

- **GET** - client requests to get resources from server i.e. open a new webpage
- **POST** - client requests to send new data to a server i.e. a tweet
- **PUT** - client requests to update existing information on server i.e. changing profile pic
- **DELETE** - client sends request to delete existing data from server i.e. deleting a post

### Anatomy of an HTTP Method

GET/HTTP/1.1.
- Method/Path/version of the protocol
Host: developer.mozilla.org
- Headers

## Status Codes

- Part of an HTTP response that gives client an idea of what happened to the request
- 3 digit numeric code

### Anatomy of a Status Code

HTTP/1.1 200 OK
- Version of the protocol, status code, status message
Date: ...
Server: Apache
- Headers

### Types

**Each code begins with number to represent the type

1. Information
2. Successful
3. Redirect
4. Client errors
5. Server errors

## Make an HTTP Request

### CLI

- cURL: like a web-browser

### GUI

- Postman
