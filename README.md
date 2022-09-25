# AJAX-example
This is made to physically demonstrate to people how Asynchronous API requests are made

Before we try to understand Asynchronous Javascript, we should first understand Synchronous Javascript.
Synchronous Java script simply means that the code is executed line by line in the order that was defined
in the code. This can create alot of problems if a line of code takes too long to execute ( For example an
alert window in Javascript is an example of a blocking task because it will stop all execution of the code
until the alert window is closed).
The solution to this is to use Asynchronous code, which simply means to execute a task after a background
process has finished execution, or we can say that the execution of asynchronous code is deferred to the 
future until the current background task is completed, then the asynchronous task is executed.

This project visually demonstrates how this takes place in practice


![image](https://user-images.githubusercontent.com/48489611/192135926-0a678bb0-4ffe-45e5-ad6d-1821388c5c64.png)



This image shows the order of execution of a function that makes API requests to a web server, then returns information
about said countries.
The order is Egypt, Germany, Canada


![image](https://user-images.githubusercontent.com/48489611/192136058-01234419-d3ee-4ce0-987e-8e025e6b8075.png)


The image above clearly shows the correct order specified in the code, however that might not always be case, the
response for the germany request may have come first or third, to test this out we can simply refresh the page to 
see the following


![image](https://user-images.githubusercontent.com/48489611/192136122-233f6d06-6368-4b2d-bf31-dccbc7859724.png)

The order in here is completely reversed, and the reason being that the order in which the response came back has 
varied.
Hopefully this was a concise and informative description of how Asynchronous Javascript works.
Feel free to clone the code and run it for yourself.
