## Console Errors ##

<aside class="notice">You might encounter errors when accessing the REST API. These console errors warn you when a variable is not defined or the script is used the wrong way. You can view them when you have developer mode enabled on your choice of browser.</aside>

Error Code | Error Type
---------- | -------
`RJ-101` | Script can not run as a file.
`RJ-102` | Authorization method was not specified.
`RJ-103` | Password for authorization is missing! (Basic authentication only.)
`RJ-104` | Namespace is unknown!
`RJ-105` | Author was not defined when creating new post!
`RJ-403` | Form method was not set. Are we posting or getting something?
`RJ-404` | Post data is empty! We kind of need data to post.
`RJ-500` | Endpoint is unknown!

Errors return both the appropriate status code followed by the response.
