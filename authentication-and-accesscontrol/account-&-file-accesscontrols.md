### Account Access Controls

user account - limited in access. cannot install, only perform tasks that admin allows for a user account to do
Admin - create, delete and handle privileges

# Types of admin

Privilege account - Type of admin account handling privilege. It is good practice to have different admin accounts for the various admin purposes, so if one is commpromised it doesn't encompass the whole thing
Service - Running services


Sponsored guest account - temporary, mayhaps for guests of the business
Shared account  - multiple users that are working on the same task, hard to identify and track who exactly is using the account
Generic account - Default from facotry, should change immediately


Accounts are associated to people, so tracking them typically looks at:
Usernames and SID ( security identifier ) - unique number


### File access control

So we have covered accounts, but what about files? How are files managed in terms of access?

On windows, we have file permissions:
Full control, modify, read and exexute, read and write, and special

Linux we have numbers = these numbers will be:
4 - reading
2 - writing
1 - executing

number 1 - owner - 7 = sum of 4,2,1 so all permissions
number 2 - group - 2  = writing
number 3 - rest of users - 3 = writing and executing
