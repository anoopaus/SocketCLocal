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
### (For the Server side!)
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
### Let's see the libraries one by one.
The header file is responsible for the standard input-output header file. Ir provides declarations for functions and macros that are used for input and output operations in C. Some of the functions such as 'scanf()','fprintf()'and 'fclose()' etc.
```c
#include<stdio.h>
````

The header file is responsible for the *Standard library*. It provides the declarations for several standard functions, types, and macros that are widely used in c programming for as memory allocation, conversion, random number generation, searching, sorting, etc.

```c
#include<stdlib.h>
````

Again this header file is *Unix standard*. It provides access to various POSIX (Portable Operating system interface) operating system servers. Some functions such as 'fork()' this function create duplicates. 'exec()' exec functions run a new program by replacing the current process image with a new process image obtained from a file in the HFS (hierarchical file system) etc.
```c
#include<unistd.h>
````

The header file defines various data types used in system programming, especially in Unix-like operating systems. One of the common functions are 'size_t' Unsigned integer type used to represent the sizes of objects. and 'pid_t' Integer type used to represent process IDs.
```c
#include<sys/types.h>
````

This header file is responsible for the essential component of socket programming in C language. In other words, this is the most important header file that needs to be included so we can provide the necessary declaration for socket-related functions, constants, and data structures used for communication between processes over the network. For example, we have some *Important functions* such as 'sock_stream' this function is responsible for the implementation of the tcp's.
```c
#include<sys/socket.h>
````

Now, This header file is really important for networking programming in C, particularly for working with IP or we can say internet addresses and sockets. Mainly it works in the field of networks it has a function named 'sockaddr_in' which structure for handling IP addresses and port numbers.
```c
#include<netinet/in.h>
````

We have a basic header file named string it is used for using the funcinalty about the string link entering a string, finding the length of a string, etc.
```c
#include<string.h>
````









 

