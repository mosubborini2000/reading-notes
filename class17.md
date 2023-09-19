Spring Boot and OAuth2
This guide shows you how to build a sample app doing various things with "social login" using OAuth 2.0 and Spring Boot.
All samples are implemented using the native OAuth 2.0 support in Spring Boot.
There are several samples building on each other, adding new features at each step:

simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).

click: adds an explicit link that the user has to click to login.

logout: adds a logout link as well for authenticated users.

two-providers: adds a second login provider so the user can choose on the home page which one to use.

custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.
Creating a New Project
First, you need to create a Spring Boot application, which can be done in a number of ways. The easiest is to go to https://start.spring.io and generate an empty project (choosing the "Web" dependency as a starting point). Equivalently, do this on the command line:

$ mkdir ui && cd ui
$ curl https://start.spring.io/starter.tgz -d style=web -d name=simple | tar -xzvf -

- you can add home page, login, and logout button
- you can login by github
- you can add error message
- All of the sample apps can be easily extended and re-configured for more specific use cases, usually with nothing more than a configuration file change. Remember if you use versions of the samples in your own servers to register with GitHub (or similar) and get client credentials for your own host addresses. And remember not to put those credentials in source control! 