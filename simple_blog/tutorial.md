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
    
      <!---The header, which contains the websites title--->
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

This will serve as the header and the navigation bar.

An ```id``` is an attribute of an HTML tag that uniquely identifies an element. 

- ```<center></center>```: This is the center tag. It displays an element at the center of the page 
- ```<ul></ul>```: This is an unordered list tag. It displays a list in either bulleted, disc, or circle form.

We will then add a sidebar, which contains a search input and links to popular posts.

```
<div id = "sideBar">
  <h3>Search For:</h3>
  <input type="text" placeholder = "Search"/>
  <br/>
  <h3>Popular Posts</h3>
  <ul type="disc">
    <li class = "list"><a href="#">Lorem Ipsum 1</a></li>
    <li class = "list"><a href="#">Lorem Ipsum 2</a></li>
    <li class = "list"><a href="#">Lorem Ipsum 3</a></li>
    <li class = "list"><a href="#">Lorem Ipsum 4</a></li>
    <li class = "list"><a href="#">Lorem Ipsum 5</a></li>
    <li class = "list"><a href="#">Lorem Ipsum 6</a></li>
  </ul>
</div>
```

Next, we will add some content for the website. For our blog site, we will add a small summary of recent posts.

```
<div class="post">
  <h2>Lorem Ipsum 1</h2>
  <h4>December 14, 2019</h4>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris luctus porta turpis, et accumsan tortor tempus sed. Quisque sollicitudin eros vitae augue rutrum facilisis. Nam in velit lacinia, aliquet justo sed, sollicitudin sem. Mauris elementum orci sit amet elit accumsan ullamcorper. Fusce posuere dolor id mattis finibus. Integer ut tempor eros. Nam consectetur elit id porttitor varius. Curabitur finibus et neque sit amet aliquam. Phasellus mattis dapibus aliquet. Mauris ut enim lacinia, condimentum mauris eget, dictum felis. Suspendisse potenti. Maecenas eu massa sem. Interdum et malesuada fames ac ante ipsum primis in faucibus...<a href="#">Read More</a></p>
</div>
<div class="post">
  <h2>Lorem Ipsum 2</h2>
  <h4>November 4, 2019</h4>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris luctus porta turpis, et accumsan tortor tempus sed. Quisque sollicitudin eros vitae augue rutrum facilisis. Nam in velit lacinia, aliquet justo sed, sollicitudin sem. Mauris elementum orci sit amet elit accumsan ullamcorper. Fusce posuere dolor id mattis finibus. Integer ut tempor eros. Nam consectetur elit id porttitor varius. Curabitur finibus et neque sit amet aliquam. Phasellus mattis dapibus aliquet. Mauris ut enim lacinia, condimentum mauris eget, dictum felis. Suspendisse potenti. Maecenas eu massa sem. Interdum et malesuada fames ac ante ipsum primis in faucibus...<a href="#">Read More</a></p>
</div>
<div class="post">
  <h2>Lorem Ipsum 3</h2>
  <h4>October 20, 2019</h4>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris luctus porta turpis, et accumsan tortor tempus sed. Quisque sollicitudin eros vitae augue rutrum facilisis. Nam in velit lacinia, aliquet justo sed, sollicitudin sem. Mauris elementum orci sit amet elit accumsan ullamcorper. Fusce posuere dolor id mattis finibus. Integer ut tempor eros. Nam consectetur elit id porttitor varius. Curabitur finibus et neque sit amet aliquam. Phasellus mattis dapibus aliquet. Mauris ut enim lacinia, condimentum mauris eget, dictum felis. Suspendisse potenti. Maecenas eu massa sem. Interdum et malesuada fames ac ante ipsum primis in faucibus...<a href="#">Read More</a></p>
</div>
```

To finish up the webiste, we will add a footer. Footers can contain links to social media accounts, site maps, and a copyright symbol. For our website, we will add a copyright symbol.

In order to create a footer, the footer tag is needed:

```
<footer>
  <h4 style="margin-left: 40px;">&copy; Copyright 2019</h4>
</footer>
```

Open ```index.html``` file to see your changes.

### My Simple Blog Site: Coding the About Page

For the About page, it looks almost the same as the Home page except with few contents.

#### Step 1: Copying the Home page's Layout
First, create a new file and name it as ```about.html```. Copy the following code and put it inside the file:

```
<!DOCTYPE html>
<html>
  <head>
    <title>My Simple Blog Site</title>
    <link rel="stylesheet" href = "site.css"/>
    <link href="https://fonts.googleapis.com/css?family=Montserrat&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Zilla+Slab&display=swap" rel="stylesheet">
  </head>
  
  <body>
    <div id = "main-content">
      <div id = "header">
        <center><h1 style="margin-top: 100px;">My Simple Blog Site</h1></center>
      </div>

      <ul id="nav">
        <li><a href="home.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>

      <div id = "sideBar">
        <h3>Search For:</h3>
        <input type="text" placeholder = "Search"/>
        <br/>
        <h3>Popular Posts</h3>
        <ul type="disc">
          <li class = "list"><a href="#">Lorem Ipsum 1</a></li>
          <li class = "list"><a href="#">Lorem Ipsum 2</a></li>
          <li class = "list"><a href="#">Lorem Ipsum 3</a></li>
          <li class = "list"><a href="#">Lorem Ipsum 4</a></li>
          <li class = "list"><a href="#">Lorem Ipsum 5</a></li>
          <li class = "list"><a href="#">Lorem Ipsum 6</a></li>
        </ul>
      </div>
      
      <footer>
        <h4 style="margin-left: 40px;">&copy; Copyright 2019</h4>
      </footer>
    </div>
  </body>
</html>
```

This is to ensure that the layout is the same as the Home page.

#### Step 2: Add a Simple About Me Content
Just above the footer tag, add this code:

```
<div id="about">
  <h2>About Me</h2>
  <img src="images/profile.jpg" width="300" height="200"/>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris luctus porta turpis, et accumsan tortor tempus sed. Quisque  sollicitudin eros vitae augue rutrum facilisis. Nam in velit lacinia, aliquet justo sed, sollicitudin sem. Mauris elementum orci sit amet elit accumsan ullamcorper. Fusce posuere dolor id mattis finibus. Integer ut tempor eros. Nam consectetur elit id porttitor varius. Curabitur finibus et neque sit amet aliquam. Phasellus mattis dapibus aliquet. Mauris ut enim lacinia, condimentum mauris eget, dictum felis. Suspendisse potenti. Maecenas eu massa sem. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin laoreet sem eget sollicitudin mollis.</p>
   <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris luctus porta turpis, et accumsan tortor tempus sed. Quisque sollicitudin eros vitae augue rutrum facilisis. Nam in velit lacinia, aliquet justo sed, sollicitudin sem. Mauris elementum orci sit amet elit accumsan ullamcorper. Fusce posuere dolor id mattis finibus. Integer ut tempor eros. Nam consectetur elit id porttitor varius. Curabitur finibus et neque sit amet aliquam. Phasellus mattis dapibus aliquet. Mauris ut enim lacinia, condimentum mauris eget, dictum felis. Suspendisse potenti. Maecenas eu massa sem. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin laoreet sem eget sollicitudin mollis.</p>
</div>
```

- ```<h2></h2>```: This is Heading 2 tag. There are 6 heding tags, with Heading 1 being the largest and Heading 6 being the smallest.
- ```<img/>```: This is the Image tag. It is an empty element, where it doesn't require the tag to be closed. The ```src``` attribute refers to the file path where the image is stored. Meanwhile, the ```width``` and ```height``` attributes are used to define the width and height of the image.

