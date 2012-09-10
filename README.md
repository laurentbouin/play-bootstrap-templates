play-bootstrap-templates
========================

Use  simple templates based on [Bootstrap for Twitter](http://twitter.github.com/bootstrap/) within your Play! applications.

Version
----------

The module uses the same [Bootstrap for Twitter](http://twitter.github.com/bootstrap/) version number.


What's inside ? 
---------------

* [Bootstrap for Twitter](http://twitter.github.com/bootstrap/) Version 2.1.1
* [JQuery](http://jquery.com) - latest version
* Two templates for your Play! applications:

###Basic template

![template](https://github.com/laurentbouin/play-bootstrap-templates/raw/master/documentation/img/template.png)

###Template with left menu

![template-leftMenu](https://github.com/laurentbouin/play-bootstrap-templates/raw/master/documentation/img/template-leftMenu.png)

Installation
------------

In your `dependencies.yml` add the module

    require
        - play-bootstrap-templates -> bootstraptemplates 2.1.1    

As `play-bootstrap-templates` is not in the Play! Repository, add a new repository in `dependencies.yml`

            
    - github-lbo:
        type:       http
        artifact:   "http://cloud.github.com/downloads/laurentbouin/play-bootstrap-templates/[module]-[revision].[ext]"
        contains:
            - play-bootstrap-templates -> *   


Usage
-----

In your `index.html` file replace `#{extends 'main.html' /}` by: 

`#{extends 'boot-template.html' /}` for the basic template

`#{extends 'boot-template-leftmenu.html' /}` for the template with the left navbar


To use the `About` and `Contact` links in the navbar simply add routes for them in your application: 

    GET 	    /about    	        Application.about
    GET 	    /contact            Application.contact


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


How to modify the top navbar
-----------------------------

* Copy the file `/modules/bootstraptemplate/app/views/tags/navbar.html` into `YOUR_APPLICATION/app/views/tags/navbar.html`
* Modify it, enjoy !  

