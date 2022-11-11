# Post Request Test README

I wanted to see how to make a post request to a server. To do this I created an app using express where the client will send a post request to the server asking for the time, and then the server will send back the time, and the client will display this on the page. 

## Challenges

1. Having the client constantly send post requests to the server, without it killing the browser

This was achieved by creating an async function called timer that returns a promise after 500ms, the while loop that is asking for the time will then await the response of timer, thus giving a 500ms delay to each request. 
