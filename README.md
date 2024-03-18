# Creating chat room using C (Socket Programming).
### What does this chatroom do?
So basically this chatroom there will be two main components a *Server* and *Client*.<br>
The server is responsible for connecting the client to the chatroom. And manage the client activity and data flow.
The client is said to be a user Who is chatting.
### Now let's know about the working principle of This Chatroom.
Socket programming is a way of connecting two nodes on a network to communicate with each other. In the context of a chatroom, the basic working principle involves the use of sockets to establish connections between the clients (users) and the server, enabling real-time communication between them.  
## Prerequisites:
As this code is for Linux and iOS-based operating systems so, to create the above project you needed.<br>
--->A Linux or ios Operating system.<br>
--->With gcc compiler.<br>
--->Intermediate knowledge of c language.<br>
The above things will be more than enough<br>
## Let's Start with the project.
Now you have to create a C file name "Server. c". With the help of the terminal.<br>
To create the file type:
```terminal
gedit Server.c
````
This will open a file and here we write out the code of socket programming in c language.<br>
So, For creating sockets and getting client requests we need to use some of the libraries of C language.
Such as:
```c
#include<stdio.h>
#include<stdlib.h>
#include<unistd.h>
#include<sys/types.h>
#include<sys/socket.h>
#include<netinet/in.h>
#include<string.h>
````
I will explain the use of these libraries one by one.




 

