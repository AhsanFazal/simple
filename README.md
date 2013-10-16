# Simple Wordpress slicing boilerplate

This repository is my personal starting point for creating Wordpress templates. Basically, it is a very simple version of the [HTML5 Boilerplate](http://html5boilerplate.com/)

To give you an better understanding of the structure of this repo you need to know how I work:

* So that I don't need to go through the trouble of having to set up a web server and a Wordpress test installation for the initial slicing process of the design, I develop in raw HTML.
* When I finished my HTML and CSS magic, I convert all the files to `.php` and use a small bash script to strip the header and footer parts from the template files.
* I upload the stuff to our development server and start implementing the Wordpress-tags.

## Template structure
Wordpress templates have a standard structure for file names, but not for the folders inside a template. I use the following structure: 

### Main folder
The main folder contains the following files:

* style.css - The main stylesheet for the project
* index.html - The base HTML file for the template, which will be later split into (at least): index.php, header.php, footer.php

Then there are four folders:
* **css/** contains all the extra stylesheets, for example normalize.css and any styles that are page-specific or required by a certain Javascript library or script.
* **js/** contains all Javascript files, of course.
* **inc/** contains all PHP files required by the template, other than the template files themselves.
* **img/** contains all images for the template.