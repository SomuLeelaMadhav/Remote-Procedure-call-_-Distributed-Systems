# Multithreaded File server Program

* This program includes source code for the client side and server side application named **client.cpp** and **server.cpp**.
* The program implements a multithreaded file server that supports upload, download, delete and rename file operations.
* It creates the connection between the client and server in which they negotiate the operation to be perfomed and can do file transfering.
* It also includes the computation server to support Add(i,j), sort(arrayA).
* The computational server also provides a set of predefined RPC that can be called from a client.

## Instructions for the program execution
* Install gcc in your computer. Open terminal and use the command 'sudo apt-get install gcc-10 g++-10'.

### Installing server
* Change the directory to where the files are located. The command 'cd <directory/filename>'
* Once in the directory, type the command 'g++ -std=c++11 -o ser server.cpp' and click enter.
* Type the command './ser' and press enter. this executes the server application, the server now awaits instruction from the client side

### Installing client
* Open a new tab in terminal
* Change the directory to where the files are located. The command 'cd <directory/filename>'
* Once in the directory, type the command 'g++ -std=c++11 -o ser client.cpp' and click enter
* Type the command './ser <command> <filename> , example ./ser upload t.txt
* On the server side it will indicate 'Recieve file:t.txt'


## Sending Instructions from the Client to the Server
1. Typing ./cli upload <filename> will upload a file currently on the client folder to the server folder.
2. Typing ./cli download <filename> will download a file currently on the server folder to the client folder.
3. Typing ./cli delete <filename> will delete the file specified currently on the server folder.
4. Typing ./cli rename <filename1> <filename2> will rename a file specified in <filename1> on the server folder to the name specified in <filename2>.
5. To execute one of the rpc commands, type rpc after the name of the executable and then follow it with the specific command.
6. Typing ./cli rpc calculate_pi will return the value of pi from the server.
7. Typing ./cli rpc add will prompt the user to enter two numbers. Simply type the two number with space between them and the result will be sent by the server on pressing enter.
8. Typing ./cli rpc sort will prompt the user to enter an array. Simply type the array elements with spaces between them and the sorted array will be sent by the server on pressing enter.
 
