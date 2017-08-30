# amon.github.io 
The Amon theme is just another project from Jorge AML using bootstrap, as you can see in the link above or here: [Amon theme](https://jorgeaml.github.io/amon.github.io/) I change a lot of colours and environment of the basic template of bootstrap because the Amon theme it's thinking to use in the night. 
Right now I am gonna explain what changes I did in this new theme: 
**all the new styles are in css/theme-aml/asphalt.css**
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
the *list-group-item-aml* has a new *display* code that is *block* I use this property because I need an the element generates a block element box.
