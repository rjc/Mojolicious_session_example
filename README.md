# Mojolicious session example
A simple Mojolicious application example for authenticating a user and maintaining a session.

This example will show you how to 
* [set up](docs/Getting_Started.md) a Mojolicious application
* create a [login page](docs/Login.md)
* add simple [authentication](docs/Authenticate.md)
* re-direct to a landing page on successful login
* return to login page with message on failed login
* where to place pages that require authenticated access
* restrict access to protected pages using [session cookies](docs/Sessions.md)
* where to place pages that are publically accessible
* add authentication via [LDAP](docs/LDAP.md)
* write to a [logfile](docs/Logging.md)

if we get time we will show you how to
* re-direct to previous page after successful authentication
* create a logout link and place it on your templates
* use a config file to store system values
* add a plugin module, such as Mojolicious::Plugin::OAuth2 and configure it

Instructions on how to build this application are found in **docs/**.
The first step is in [Getting_Started](docs/Getting_Started.md).
