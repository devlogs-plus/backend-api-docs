# Backend API Docs

These are the http requests for the backend API. This is not a publicly accessible API.

## HTTP Requests

The http requests each have a comment on the top, the type of request (GET, POST, etc.), and the url. 
If a request needs a JSON body the file includes what the api expects.
The request ends with triple hashtag: ###

Here is an example of a request
```http request
### this does stuff
POST {{BASE_URL}}/auth/resetpassword
Content-Type: application/json

{
    "thing1": "string",
    "ting2": 1,
    "thing3": "waow"
}

###
```

## Organization

The .http files are organized into different folders. 
The auth folder holds all the auth requests
The devlogs folder holds all requests relating to devlogs, creating, editing, publishing, and more.
The projects folder has all the project requests, creating, viewing, getting them, etc.
And finally, the time folder has all the requests for time tracking.
The only lone request is the feed.http which is there because it doesnt really fit anywhere else.