Task 1.
In a telecommunications network, data transfer occurs using two protocols A, B. However, information has appeared that a third protocol C has begun to be used for data transfer.
After some time and through incredible efforts, it was possible to obtain a data set (dataset) of sessions of this protocol. Moreover, it was possible to detect this protocol with a high probability.
But the problem is that when working simultaneously, the quality of information transmission suffers, and it is very important that Protocol A functions without loss of quality.
Therefore, it is necessary to separate the traffic of different protocols. Our valiant engineers began to solve the problem and even generated data sets with examples of sessions of the above protocols.
They even decided to study what information was transmitted using the C protocol, and realized that this was some kind of gobbledygook.
But they weren’t enough for more, and while they were collecting traffic they were often distracted by other tasks. In general, at some point, they got tired of this activity and quit in unison,
leaving as a curse a file in pcapng format and a dataset containing packets of sessions of all protocols that they had not yet managed to parse. So it’s impossible without your help. 
And we will hire those who show themselves in the best way (instead of these quitters).

Given: 1) Datasets containing session data of protocols A, B and C.
       2) Files in pcapng and csv format containing session packets of all protocols.
       
Required: Implement an algorithm for classifying protocol sessions that does not reduce the quality of transmission of protocol A sessions and leaves the possibility of using protocol B.
Test the implemented algorithm on an unclassified dataset (.csv file). As a solution, propose a resulting dataset that consists of session string indexes (in the sequence in which they are present in the original dataset)
and the assigned protocol name (“A”, “B”, “C”)


Task 2.

The network engineers who left us decided to come back. But this time we decided to entrust them with another job (after all, now we have you).
The fact is that we have put into operation a new communication line and want to understand how many different protocols transmit data over it.
The guys completed the work and created two datasets with sessions of different protocols. But we remember how they approach the matter and decided to check their work.
And since we have no one else to rely on, you have to perform this check and create datasets based on the true number of protocols. And then we’ll decide whether to fire these guys or let them work.

Given: Two datasets, each containing session data of different protocols and one unsorted dataset.

Required: make sure that each dataset contains session data of only one protocol. If this is not the case, then provide the true number of protocols and the session numbers belonging to each protocol.
As a solution to the task, present the true number of different protocols contained in the original datasets. Also provide datasets on the number of protocols.
Each dataset contains records containing line numbers of the unsorted dataset, belonging to sessions of the same protocol (each dataset contains only line numbers with sessions of the same protocol).


Task 3.

We have problems again. It turned out that our security specialists missed the moment when users began visiting illegal resources disguised as legal ones. 
We have fixed the security issues, but now to conduct a successful investigation (and identify those responsible), we need to determine at what point users began visiting spoofed resources. 
Luckily, we still had traffic records in the form of moments in time when requests were sent to the server. We were also able to find out that the intensity of requests to the legal and spoof servers differs. 
And again you have this difficult but honorable work ahead of you.

Given: Datasets representing information about the time of sending requests to the server, which may contain the moments of transition to replacement resources

Required: To most accurately determine the moment when users switch to replacement resources. As a solution, you need to provide the time in seconds from the beginning of the dataset when users switched to substitute resources.
