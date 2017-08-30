# amon.github.io 
The Amon theme is just another project from Jorge AML using bootstrap, as you can see in the link above or here: [Amon theme](https://jorgeaml.github.io/amon.github.io/) I change a lot of colours and environment of the basic template of bootstrap because the Amon theme it's thinking to use in the night. 
Right now I am gonna explain what changes I did in this new theme: 
**all the new styles are in css/theme-aml/asphalt.css**

### Before we get started

I just to remember to install bootstrap on your desktop, so you have RubyGems and adding the following line to your GemFile:
```
gem 'bootstrap', '~> 4.0.0.alpha6'
```
Alternatively, if you’re not using Bundler, you can install the gem by running this command:
```
gem install bootstrap -v 4.0.0.alpha6
```
or make it simply, download the source code at [getbootstrap](https://github.com/twbs/bootstrap/releases/download/v4.0.0-beta/bootstrap-4.0.0-beta-dist.zip)

## Using a CDN

Or another way skip the download with the Bootstrap CDN to deliver the cached version of Bootstrap’s compiled CSS and JS to your project.
```
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta/css/bootstrap.min.css" integrity="sha384-/Y6pD6FV/Vv2HJnA6t+vslU6fwYXjCFtcEpHbNJ0lyAFsXTsjBbfaDjzALeQsN6M" crossorigin="anonymous">
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta/js/bootstrap.min.js" integrity="sha384-h0AbiXch4ZDo7tp9hKZ4TsHbi047NrKGLO3SEJAg45jXxnGIfYzk4Si90RDIqNm1" crossorigin="anonymous"></script>
```
If you’re using our compiled JavaScript, don’t forget to include CDN versions of jQuery and Popper.js before it.
```
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.11.0/umd/popper.min.js" integrity="sha384-b/U6ypiBEHpOf/4+1nzFpr53nxSS+GLCkfwBdFNTxtclqqenISfwAzpKaMNFNmj4" crossorigin="anonymous"></script>
```
## the CSS asphalt on Amon

1. navs 
the new style of the navs has a new style that is a background, border-bottom and a box-shadow. you need to know what changes are: 
``` asphalt.css
background-colour: #1a2636;
border-bottom: 4px solid #2a4d69;
box-shadow: 0px 1px 1px 1px #0e1a40;
```
2. **class aml_banner**
This  class have a *margin-top of 2%*  because navs have a new height, so when you need to create a new object after navs, your new object always will be in the back not in the front and your object are in up more of the limit of your nav so that reasons I set in asphalt.css: 
```
margin-top: 2%;
left: 0;
```
You can use the class **aml_banner** when you create a new object or a new div in your HTML.

3. class **list-group-aml*** and ***list-group-item-aml***

obviously is the same class in bootstrap but with the *aml* code, this class I recommend to use with a *container-fluid* and a *col-sm-3* you can use with up to 4 or 5 but I not recommend a *col-sm-6* or *col-md-6* because it won't be a list, you will be like a large container and you lost the complex of the container.
the *list-group-item-aml* has a new *display* code that is *block* I use this property because I need the element generates a block element box.

this new property has:
```
.list-group-aml {
    background-color: #142842;
    margin-bottom: 5%;
    border: 4px solid #2a4d69;
    border-radius: 5px;
}
.list-group-item-aml {
    color: #e7eff6;
    display: block;
    padding: 3%;
    border-bottom: 1px solid #2a4d69;
}
.list-group-item-aml:hover {
    color:     #ff9900;
    background-color: #002448;
    text-decoration: none;
}
```
