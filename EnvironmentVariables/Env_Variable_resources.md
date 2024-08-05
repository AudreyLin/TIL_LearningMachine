# Environment Variables

### What is an environment variable 

An environment variable is a variable that sets a value (using a name-value pair syntax) to use for reference within an operating system or program that influence the behavior and interactions with other processes within the operating system or program environment and scope(s) when they are called by name by using the value in its place. 

### What are environment variables used for?

It is typically used to ensure consistency within a large program to ensure that no bugs, typos, or missed implementations are had within a program's configuration.  Initially, it would be fine to ensure everything works at testing.  However, after the code is written, if it has many files, it is hard to find all the places in code that refer to a certain configuration.  So, environment variables allow you to reference the configuration data throughout the code base, and if the data changes you can just change it in the set environment variable instead all throughout the codebase. This saves time and prevents the need to sort through and alter all of the code, then having to retest, and redeploy everything.  It also prevents unwanted side effects in production.  

### Use Cases for environment variables

* Execution modes (IE: production, development, testing, staging,etc)
* Domain Names
* API URL/URI's
* Authentication Keys
* group mail addresses
* service account names
* Information that needs to be secure & controlled in a single place to reduce risk of leaking important data


## Resources
- [Intro to Environment Variables](https://medium.com/chingu/an-introduction-to-environment-variables-and-how-to-use-them-f602f66d15fa)
- [Environment Variables Explained](https://www.dreamhost.com/blog/environment-variables/)
- [Environment Variables OpenGroup](https://pubs.opengroup.org/onlinepubs/009695399/basedefs/xbd_chap08.html)
- [GeeksForGeeks: Linux Env_Variables](https://www.geeksforgeeks.org/environment-variables-in-linux-unix/)