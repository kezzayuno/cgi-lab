# CMPUT404 CGI Experiments

Experimenting with CGI server stuff!

Question 1: How do you inspect all environment variables in Python?

os.environ

Question 2: What environment variable contains the query parameter data?

QUERY_STRING (can be seen in the URL as ?q=)

Question 3: What environment variable contains information about the user’s browser?

HTTP_USER_AGENT

Question 4: How does the POSTed data come to the CGI script?

s = cgi.FieldStorage() # form which stores the username and password input
username = s.getfirst("username")
password = s.getfirst("password")

Question 5: What is the HTTP header syntax to set a cookie from the server?

Set-Cookie: 

Then, you put the variable you want to save (username, for example) and the input: "username=inputted_username"

Question 6: What is the HTTP header syntax the browser uses to send the cookie back?

HTTP_COOKIE

Question 7: In your own words, what are cookies used for?

Cookies are used to save previous inputted data from the user. 

Question 8: What is the link to your code on GitHub?

https://github.com/kezzayuno/cgi-lab
https://github.com/kezzayuno/cgi-lab.git

