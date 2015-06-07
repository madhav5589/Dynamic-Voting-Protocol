1) The Source Folder contains Source Code for Server and Client Folder contains Source Code for Client.
2)CompileAll.sh is used to compile and run the Server or Client Code in the respective folders for Server and Client.
3)Use dc11-dc17 for Server and dc21-dc25 hosts for Client.
4)There are folders server1,server2,server3...Server7 in the folder Server.Each Server folder mains three Objects appropriately.
4)First start the Servers on dc11-dc17 by running the command './CompileAll.sh'
5)After all the Servers are ready and listening on a port 1234.
6)Initialize all the clients one after one from dc21 to dc25.
7)You can see the Clients and Servers Communicating and Clients writing to Objects by a two phase Communication.
8)The log files Client1.txt-Client5.txt are available in the CLient folder
9)The Objects can be checked for synchronizationa at the end of the 20critical Sections by using a 'diff Server1/Object1.txt Server2/Object1.txt'.