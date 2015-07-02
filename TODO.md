# List of things To Do

* add a test to show morbo is working 00_getting_started.t

## Login

* add a login page to the app that has Username and Password fields
* show the changes required to add the route and a template
* add a test for login success and failure 01_login.t

## Protected Pages

* add open pages to a route under open/* - pages that can be seen without logging in
* add a test 02_open_pages.t
* add protected pages to a route under protected/*
* add a test 03_protected.t
** should redirect to login page on accessing protected/* without logging in
** like to remember where it came from so that on success it can return to

## Logout

* add a Logout button to attach to a template or layout
* add a test 04_logout.t to check successful logout and can't access protected/*