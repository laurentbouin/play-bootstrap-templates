play-bootstrap-templates
========================

Use  simple templates based on [Bootstrap for Twitter](http://twitter.github.com/bootstrap/) within your Play! applications.

Version
----------

The module uses the same [Bootstrap for Twitter](http://twitter.github.com/bootstrap/) version number.


What's inside ? 
---------------

* Bootstrap for Twitter Version 2.1.1
* JQuery - latest version
* Two templates for your Play! applications:

###Basic template

![template](https://github.com/laurentbouin/play-bootstrap-templates/raw/master/documentation/img/template.png)

###Template with left menu

![template](https://github.com/laurentbouin/play-bootstrap-templates/raw/master/documentation/img/template-leftMenu.png)

Installation
------------

Usage
-----

In your `index.html` file change `#{extends 'main.html' /}` by: 

`#{extends 'boot-template.html' /}` for the basic template
`#{extends 'boot-template-leftmenu.html' /}` for the basic template


I18N
----

Add the following messages:

    title=Home
    navbar.home=Home
    navbar.about=About
    navbar.contact=Contact
    project.name=My Project
    footer.company=&copy; MyCompany 2012

How to modify the left navbar
-----------------------------

* Copy the file `/modules/bootstraptemplate/app/views/tags/leftMenu.html` into `YOUR_APPLICATION/app/views/tags/leftMenu.html`
* Modify it, enjoy ! 

