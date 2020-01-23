# Creating a Three Page Simple Blog Site

### Overview
In this tutorial, we will be creating a three page blog website. The pages will include: the home page, about page, and a contact page.

#### Resources needed

Images used: https://github.com/AndreaGon/website_projects/tree/master/simple_blog/images

### My Simple Blog Site: Coding the Home Page

#### Step 1: Setting up the working environment
Before starting to code, create a folder and name it as simple_blog. This will be the website's folder. 

#### Step 2: Adding the Head

HTML doesn't need an IDE or a coding editor for it to run. A simple text editor (Notepad) can be used to write HTML and CSS.

On your Text Editor, type in this code:

```
<!DOCTYPE html>
<html>
  <head>
    <title>My Simple Blog Site</title>
    <link rel="stylesheet" href = "site.css"/>
    <link href="https://fonts.googleapis.com/css?family=Montserrat&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Zilla+Slab&display=swap" rel="stylesheet">
  </head>
```
What does this mean?
- ```<!DOCTYPE html>```: It tells the web browser what version of HTML we are using. Currently, we are using HTML 5
- ```<html></html>```: It is where all the HTML elements are contained.
- ```<head></head>```: The head tag is the container for the head elements. Head elements include the title, the linked style, the meta information, and more.
- ```<title></title>```: Displays the title of the web page in the title bar.
- ```<meta charset="utf-8"/>```: It specifies how each character will be encoded.
- ```<link rel="stylesheet" type="text/css" href="site.css"/>```: This links the external CSS file.
- ```<link href="https://fonts.googleapis.com/css?family=Montserrat&display=swap" rel="stylesheet">```: This is a generated link from Google Fonts

Save the file as ```index.html```.


#### Step 3: Adding the Body

Below the ```<head></head>```, add this lines of code:

```
 <body>
    <div id = "main-content">
      <div id = "header">
        <center><h1>My Simple Blog Site</h1></center>
      </div>

      <!---Navigation bar--->
      <ul id="nav">
        <li><a href="home.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </div>
 <body>
```

An ```id``` is an attribute of an HTML tag that uniquely identifies an element. 

- ```<center></center>```: This is the center tag. It displays an element at the center of the page 
- ```<ul></ul>```: This is an unordered list tag. It displays a list in either bulleted, disc, or circle form.

