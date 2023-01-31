# CSE 15L Week 2 Lab Report
## Part 1- StringServer
I used the NumberServer.java file from the Week 2 Lab as the basis for my StringServer code, refining different parts to better fit the prompt. 
Here is the code for my StringServer:
<img width="1011" alt="Screen Shot 2023-01-30 at 4 36 54 PM" src="https://user-images.githubusercontent.com/122496338/215628698-06e82ee7-d587-4795-acd8-9b2293572174.png">
<img width="932" alt="Screen Shot 2023-01-30 at 4 37 24 PM" src="https://user-images.githubusercontent.com/122496338/215628714-2ba18ef1-fe7a-42ad-a1de-e5b44f9cb022.png">

Starting with an empty string and an empty String ArrayList, the conditional checks if the path is simply a "/", in which case it returns a list containing all the strings added to the web server. If the path contains "/add-message," the string following the "=" sign in the query is added to the list and displayed on a new line. In addition, the class StringServer ensures that any port the web server is called to be hosted on is a valid port number. If it is not a valid port, or a port is not present, the user is prompted to request another port number. 
