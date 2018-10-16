# Distributed Systems and their Features
## Case Nr. 1
A server program written in one programming language (for example C++) provides the implementation of a BLOB (Binary Large Object) object that is intended to be accessed by clients that may be written in a different language (for example Java). The client and server computers may have different hardware, but all of them are attached to an internet.

###### *Question*
Describe the problems due to each of the five aspects of heterogeneity that need to be solved to make it possible for a client object to invoke a method on the server object.

###### *Answer*
The computer can be make differently. For this we need to try to understand the difference between two data elements in custumer tasks and reply messages from client to objects. So we need to define a standart for each type of data item. 
The computer can run different operating system. For exemple with VirtualBox or a Bootcamp. For that Java or C++ can be very usefull, because we can use a common operation wich will be translate for each operating system where it is runing.
But we need to define some standart between C++ and Java, because there are different in lots of aspect and they are Two different langage. But with this standart we can creat a translation. It is possible that we have different implementors for exemple C++ and Java. They must creat some common standart together.


## Case Nr. 2
###### *Let us contunue with a situation from Case Nr. 1*
An open distributed system allows new resource sharing services such as the BLOB object mentioned in Case Nr.1. 
to be added and accessed by a variety of client programs. 

###### *Question*
Discuss in the context of this example, to what extent the needs of openness differ from those of heterogeneity.

###### *Answer*

For the heterogeneity we need to respect the standart that we spoke just upper.
But for the openness differ it s different. We need to accept the standart before the BLOB object was implemented. The implementor must be respect this standart. Morover, the custumer must have access of the interface to the BLOB object. This publication is an obligation, if we want the implementation of the part of this system and if we want want that they work together.

## Case Nr. 3
###### *We are working with a relevance to situation from Case Nr. 1 about BLOB*
Suppose that the operations of the BLOB object are separated into two categories – public
operations that are available to all users and protected operations that are available only to certain
named users. 
###### *Question*
State all of the problems involved in ensuring that only the named users can use a
protected operation. Supposing that access to a protected operation provides information that
should not be revealed to all users, what further problems arise?

###### *Answer*

The problems are:
-Defining identities of the users.
-Identity theft. Some peaple can said that he is a person but in reality he is not this person.
-preventing the fake user to do some bad action with request message of the real user.
-the private information of one user must be hidden from other user. To hide this message we need to encrypte this last.
