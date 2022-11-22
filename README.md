In this project, I was solving the following problem: how to find a way to query the list of documents to create a list of employees in a company. Also, how to add new documents and how to query the updated list in the fastest way possible.

There were several types of documents available in the sample. The ones that we are going to focus on are:
-  Job Offer 
-  Company Agreement and Employment Agreement
-  Company Addendum and Employment Addendum
-  Resignation Notice and Resignation Confirmation


First, a Job Offer is created. Offered position is specified there. Then, if the candidate agrees, a pair of Candidate Agreement and Employment Agreement is created. Later, if an employee's position changes, Company Addendum is created. If that employee agrees, Employment Addendum is created. If an employee decides to resign, first Resignation Notice, than Resignation Confirmation is created, specifying the last working date. 

We chose the following approach: use Neptune database to store the documents, pulling the necessary characteristics from .jsonld representation, and then query the derived graph. 
