## Spring Boot and OAuth2

steps to create sample app has Oauth with spring boot

note:  the outdated jQuery library I'll never be used after 2016, easier to build API and use react or vue as front end 

* simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).

* click: adds an explicit link that the user has to click to login.

* logout: adds a logout link as well for authenticated users.

* two-providers: adds a second login provider so the user can choose on the home page which one to use.

* custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.

the rest of reading how to setup the code and start with a single-page app and link it with GitHub, how to get each endpoint and use jquery with it, and how to use js-cookie in your web app, and if you get a bad request how to handle that build own Bean.


We've seen how to utilize Spring Boot and Spring Security to quickly construct apps in a variety of styles. Authentication using an external OAuth 2.0 provider is a common thread running across all of the demos. All of the sample apps may be readily extended and re-configured for more particular use cases with just a few changes to the configuration files. Remember to register with GitHub (or something similar) and receive client credentials for your own host addresses if you use copies of the examples on your own servers. And don't forget to keep those credentials out of source control!
