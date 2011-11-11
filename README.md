# What is this? #

This Boilerplate is a HTML5/CSS/JS Skeleton for start a web site quickly and orderly. Contains a group of Javscript plugins and CSS/LESS styles for a rapid start of a web develpment.

It uses the tools and the file structure i've used for my projects and I think is comfortable and optimal to work with multiple platforms (Web2py, Flask, Django, CodeIgniter, etc).

This is my attempt to solve problems that occur with poor communication between designer and programmer for a lack of guidelines.


# How i use this? #

You must clone the repo and start add, edit and delete as necessary. For a best practices follow the next conventions.

## File structure and names ##

### Directories ###

Always exist a directory called static, media or assets in the project directory together with all the html files. Inside of that directory must be four directories stylesheets, javascripts, src and images.

#### Example:

```
myproject/
  static/
    javascripts/
    stylesheets/
    src/
    images/
  index.html
  page_one.html
  page_two.html
```

### Html files ###

All HTML files go in the project directory and each word of the file is separated for an underscore '\_'. 

#### Example:

```
index.html page_one.html page_two.html
```

### Stylesheets ###

All stylesheets files go in stylesheets directory into assets directory.

bootstrap.css is a compiled version of bootstrap.less.

### Javascripts ###

Exist various type of js files:

- **libs directory**: All libs like jquery, jquery-ui, plugins go here.
- **site directory**: Scripts specific for a page go here.
- **base.js**: All general functions and plugin calls go inside this file.

libs and site directories and the base.js go inside of assets directory.

### Images ###

The images directory go in to assets directory. Inside of images directory go various directorys of images for plugins/sections/groups of images.

Images names: htmlfilename\_group\_size\_name.png the htmlfilename, group or size are optional and go separated with a underscore '\_'.

### Less styles ###

Inside of src directory go all styles source with less format, in the less directory go all the sources and inside of the libs directory go de less.js for load the less styles on the fly (Read the lesscss documentation for more info.

### Json and XML test data ###

Inside of ws directory in src directory go all the test data in formta js or xml for test webservice

#### Example ####
```
              static/
                images/
                  myplugin/
                    bg_black.png
                    bg_white.png
                  header_500x200.png
                  header_500x180.png
                  btn_save.png
                  btn_delete.png
                  page_one_header_500x180_red.png
                javascripts/
                  libs/
                    jquery-1.7.min.js
                    html5.js
                    jquery.myplugin.js
                  site/
                    page_one.js
                  base.js
                stylesheets/
                  bootstrap.css
                  myplugin.css
                src/
                  less/
                    bootstrap.less
                    custom.less
                  libs/
                    less-1.1.3.min.js
                  ws/
                    data.json
                    data.xml
              index.html
              page_one.html
              page_two.html
            
```
## HTML basic structure ##
## Less and CSS style names ##
## Twitter Bootstrap ##
## Javascript, Jquery and plugins ##
## My base.js ##
## How i should make my psd/gimp template? ##



