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
myproject/
  static/
  index.html
  page_one.html
  page_two.html
```

### Stylesheets ###

All stylesheets files go inside ot the stylesheets directory into assets directory.

The **bootstrap.css** file is a compiled version of **bootstrap.less** and it contains all css styles and is required because in this file go all css style of the project.

The convention for the names of the stylesheet files for plugins and 3rd party addons is this:

framework.plugin_name.css or name_script.css

#### Example:

```
myproject/
  static/
    javascripts/
    stylesheets/
      bootstrap.css
      jquery.my_plugin.css
      some_script.css
    src/
    images/
  index.html
  page_one.html
  page_two.html
```

### Javascripts ###

Exist various type of js files all this go inside of the javascripts directory into assets and sorted into subdirectories:

- **libs ands plugins**: All libs and plugins like jquery, jquery-ui, jquery.somenthingcoolfeature go inside of the **libs** directory.
- **site scripts**: All scripts specific for a page go here in the **site** directory and the name is the same of the html file.
- **base.js**: All general functions and plugin calls go inside this file inside of the javascripts directory.

#### Example:

```
myproject/
  static/
    javascripts/
      libs/
        bootstrap-modal.js
        jquery-1.7.min.js
        jquery.form.js
        html5.js
      site/
        page_two.js
      base.js
    stylesheets
    src/
    images/
  index.html
  page_one.html
  page_two.html
```
Eduardo
sí fue para ella
 

### Images ###

The images directory go in to assets directory. In to this directory being several directories of images for plugins,sections orgroups of images.

Images names: htmlfilename\_group\_size\_name.png the htmlfilename, group or size are optional and go separated with a underscore '\_'.

#### Example:

```
myproject/
  static/
    javascripts/
    stylesheets
    src/
    images/ 
      myplugin/
        bg_black.png
        bg_white.png
      header_500x200.png
      header_500x180.png
      btn_save.png
      btn_delete.png
      page_one_header_500x180_red.png
  index.html
  page_one.html
  page_two.html
```

### Less styles ###

Into assets directory exist a directory called src, this contains some subdirectories like the src file. Into this directory go all less stylesheets files.

This less files are part of the twitter bootstrap structure in **bootstrap.less** we can indicate which files load to generate the **bootstrap.css**.

Into the **custom.less** we write the code for all css styles for our site in a less format.


### Json and XML test data ###

Inside of ws directory into src directory go all the test data in formta js or xml for test webservice. File like:

```
data_source.json other_data_source.xml
```

There files are for test APIS in a local way with a test data.


#### Example of a complete file system structure####
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

The html file must be a html5 file. The suggest structure is this.

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Boilerplate: Start here!</title>
    <meta name="description" content="Boilerplate">
    <meta name="author" content="Alvaro Lizama Molina">

    <!-- HTML5 shim, for IE6-8 support of HTML elements -->
    <!--[if lt IE 9]>
    <script src="static/javascript/libs/html5.js"></script>
    <![endif]-->

    <!-- CSS required styles -->
    <link rel="stylesheet" type="text/css" href="static/stylesheets/bootstrap.css">

    <!-- CSS optional styles -->

    <!-- LESS -->
    <!-- <link rel="stylesheet/less" type="text/css" href="static/src/less/bootstrap.less"/> -->
    <!-- <script src="static/src/libs/less-1.1.3.min.js" type="text/javascript"></script> -->
  </head>

  <body>

    <div class="container">

      <div class="content">

      </div> <!-- /content -->

      <footer>
      <p>&copy; Company 2011</p>
      </footer>

    </div> <!-- /container -->

    <!-- Required javascript libs -->

    <!-- Optional javascript libs -->

    <!-- Base javascripts for general functions and initialze plugins -->

  </body>
</html>
```
Is basic structure and the div with the class container could be fixed with a class **container** or fluid with the class **container-fluid**.

Inside **.container** could be a side bar, footer and/or content div.

```
<div class="container-fluid">
  <div class="sidebar">
    ...
  </div>
  <div class="content">
    ...
  </div>
  <div class="footer">
    ...
  </div>
</div>
```

Or you could use the grid system inside the div container. (See the Twitter Bootstrap section)

## Less and CSS style names ##
## Twitter Bootstrap ##
## Javascript, Jquery and plugins ##
## My base.js ##
## How i should make my psd/gimp template? ##



