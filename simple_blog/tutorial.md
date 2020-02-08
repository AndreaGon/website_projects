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
        <center><h1 style="margin-top: 100px;">My Simple Blog Site</h1></center>
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

Save the file and open it in a browser.

### My Simple Blog Site: Coding the Contact Page

For the Contact Page, we will create it with Forms.

#### Step 1: Copying the layout from Home Page

Like the About Page, we also need to copy the layout of the Home Page in order to be consistent.

Create a new file with the name ```contact.html``` and enter this code:

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

#### Step 2: Adding the Contact Form

Before adding the actual code to create the form, add the container first to style the elements easily:

```
<div id = "form">
   <h2>Contact</h2>
</div>
```

```<h2>Contact</h2>``` will be the header of the page.

Under Header 2, add this code for the form:

```
<form method="GET" action="mailto:emberaurelia@gmail.com">
  <label for="name">Name:</label>
  <input type="text" id ="name" name="name" placeholder="Enter your name here..."/>

  <label for="email">E-mail</label>
  <input type="text" id ="email" name="email" placeholder="Enter your email here..."/>

  <label for="mcontent">Message Content</label>
  <br/>
  <textarea rows="15" cols="10"></textarea>

  <input type="submit" id="submit" name="Submit" value="Submit"/>
</form>
```

- ```<form></form>```: This is the Form tag. It is used to create an HTML form. 

The ```method``` attribute is used to specify how to send the entered data in the form. There are two types of form-data transfer: POST and GET. The GET method appends the data in the URL, while POST has a separate file that holds the data from the form. The ```action``` attribute specifies where to send the data. 

- ```<label></label>```: The label tag is used to add a title to an element.
- ```<input/>```: There are many types of input tag, which are specified using the ```type``` attribute: checkbox, text, radio, submit, reset, password, etc.
- ```<textarea></textarea>```: The text area tag is used to create input space that can hold unlimited number of characters.

Save the file and open it on your browser.


### My Simple Blog: Adding the CSS

There are three ways to add CSS to HTML: Inline, Embedded, and External. Inline CSS requires the use of the ```style``` attribute, and is only used when you want to style a particular element. Meanwhile, embedded CSS, as its name implies, is embedded on the HTML file. It uses the ```<style></style>``` tag. On the other hand, CSS is placed on a separate file in external CSS. The CSS file is then linked to the HTML file with the use of the ```<link/>``` tag. This is best used when all of your HTML files have the same style.

#### Step 1: Styling the Web Pages with Inline and Embedded CSS

You probably noticed that inline CSS was already in used when creating the Home Page. Inline CSS was used to style ```<h1></h1>``` and ```<h4></h4>```.

We are then going to add embedded CSS to style the recenet post containers in the Home page. Inside the ```<head></head>``` tag, add this lines of code:

```
<style>
  .post{
    margin: 30px;
    margin-left: 70px;
    width: 700px;
    padding: 40px;
    background-color: #FFFFFF;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
</style>
```

This should add style to the recent post containers. 

Next, we are going to style the Contact page with embedded CSS. Add this lines of code inside the ```<head></head>``` tag:

```
<style>
  input[type=submit] {
    background-color: #D4E88E;
    color: black;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
</style>
```

This will style the submit button of the form.

#### Step 2: Creating External CSS to Style the Whole Website

First, create a new file and name it as ```site.css```. The CSS style for every web page will go here.

Add the following lines of CSS to style the body, main container, and the navigation bar:

```
/**Remove any spacing first to avoid container spacing.**/
body{
  padding: 0;
  margin: 0;
  background-color: #A6CF7E;
}

#main-content{
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  background-color: #D4E88E;
  margin: 100px;
  margin-top: 50px;
  margin-bottom: 50px;
}

/**Add Header Image**/
#header {
  display: inline-block;
  height: 300px;
  width: 100%;
  background-image: url("images/headerIMG.jpg");
  background-repeat: no-repeat;
  background-size: 100% 100%;
}

/**Style for the navigation list**/
#nav {
  list-style-type: none;
  text-align: center;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

#nav li {
  display: inline-block;
  margin-left: 40px;
}

#nav li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 14px;
  text-decoration: none;
  font-size: 150%;
}

/**When user hovers over a nav link, darken background of link**/
#nav li a:hover {
  background-color: #111;
}
```
We are also going to add style to the side bar, which includes a search bar and a list of popular posts.

```
#sideBar{
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  padding: 20px;
  position: absolute;
  right: 250px;
  margin: 30px;
  margin-right: -20px;
  background-color: #FFFFFF;
}

input[type=text] , textarea {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}

.list{
  margin: 0;
  padding: 0;
  margin-bottom: 20px;
}
```

To create unity in font styles, we have to add it in our external CSS file as well.

```
h1, h2, h3, h4{
  font-family: 'Montserrat', sans-serif;
}

p, label{
  font-family: 'Zilla Slab';
}

/**This is to style about and form container**/
#about, #form{
  margin: 30px;
  margin-left: 70px;
  width: 700px;
  padding: 40px;
  background-color: #FFFFFF;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
```
Finally, all that is left ot style is the footer.

```
footer{
  margin-top: 100px;
  width: 100%;
  padding-top: 50px;
  padding-bottom: 50px;
  background-color: #333;
  color: white;
}
```

Save ```ste.css``` and refresh the website.
