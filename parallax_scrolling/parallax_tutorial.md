# Parallax Scrolling Effect Using HTML & CSS


### Overview
A parallax scrolling is a type of web design where the background content moves at a different speed than the foreground content as the user scrolls.

##### Website without Parallax Scrolling Effect
https://www.w3schools.com/howto/tryhow_css_parallax_demo_none.htm

##### Website with Parallax Scrolling Effect
https://www.w3schools.com/howto/tryhow_css_parallax_demo.htm


#### When To Use Parallax Scrolling?
- When you want the user to scroll through your website
- The website is meant to tell a story


### Photography Portfolio: A Simple Parallax Scrolling Project

#### Step 1: Setting up the working environment
Before starting to code, create a folder and name it as Photograph_Portfolio. This will be the website's folder. 

#### Step 2: Adding the Head

HTML doesn't need an IDE or a coding editor for it to run. A simple text editor (Notepad) can be used to write HTML and CSS.

On your Text Editor, type in this code:

```
<!DOCTYPE html>
<html>
  <head>
    <title>Photography Portfolio</title>
    <meta charset = "utf-8"/>
    <link rel = "stylesheet" type="text/css" href="main.css"/>
    <link href="https://fonts.googleapis.com/css?family=Montserrat&display=swap" rel="stylesheet">
  </head>
</html>
```
What does this mean?
- ```<!DOCTYPE html>```: It tells the web browser what version of HTML we are using. Currently, we are using HTML 5
- ```<html></html>```: It is where all the HTML elements are contained.
- ```<head></head>```: The head tag is the container for the head elements. Head elements include the title, the linked style, the meta information, and more.
- ```<title></title>```: Displays the title of the web page in the title bar.
- ```<meta charset="utf-8"/>```: It specifies how each character will be encoded.
- ```<link rel="stylesheet" type="text/css" href="main.css"/>```: This links the external CSS file.
- ```<link href="https://fonts.googleapis.com/css?family=Montserrat&display=swap" rel="stylesheet">```: This is a generated link from Google Fonts

Save the file as ```index.html```.


#### Step 3: Adding the Body

Below the ```<head></head>``` tag, add this lines of code:

```
<body>
  <div class = "parallax">
    <div class = "header">
      <h1>Andrea's Photos</h1>
      <h4>Scroll for more</h4>
    </div>
  </div>
</body>
```

This will be the background container. Currently, it doesn't have background image. It only contains the headings.
- ```<body></body>```: This is where all the web contents are placed.
- ```<div></div>```: This is a division tag. It is used as a container for other HTML elements.
- ```<h1></h1>```: It defines which heading to use, with ```<h1>``` being the largest heading and ```<h6>``` being the smallest.

A ```class``` is an attribute that defines the style of elements with the same class name. We will use the class name later in CSS.

Below ```<div class="parallax"></div>```, add this line of code:

```
<div class = "foreground-container">
</div>
```
This will be the foreground container.

Under the foreground container, we will add in sample photos as contents. 
```
<h1 class = "head-sample"><u>Sample Photos</u></h1>

<!--This is to properly display the featured images-->
<table class = "table1" align = "center">
  <tr>
    <td rowspan = "2">
      <div class = "feature">
        <a href="#">
          <img src="images/sample2.jpg" class = "featured-img" height="650" width="510">
          <div class = "overlay"><div class ="text">Terrain</div></div>
        </a>
      </div>
    </td>
    <td>
      <div class = "feature">
        <a href="#">
          <img src = "images/sample1.jpg" class = "featured-img" width="550" height="330"/>
          <div class = "overlay"><div class ="text">Nature</div></div>
        </a>
      </div>
    </td>
  </tr>
  <tr>
    <td>
      <div class = "feature">
        <a href="#">
          <img src = "images/sample3.jpg" class = "featured-img" width="550" height="310"/>
          <div class = "overlay"><div class ="text">Others</div></div>
        </a>
      </div>
    </td>
  </tr>
</table>
```

Lastly, we will add in the ending container.
```
<div class = "parallax2">
  <div class = "ending" align="center">
    <h1>Want more photos?</h1>
    <h4>Check out my other platforms</h4>
  </div>

</div>
```

Save the file and run.

#### Step 4: Adding CSS to the Background Container

Create a new file and name it as main.css. Save it in the same folder with the index.html file.

We will first style the background content.
```
/**Setting the margin and padding to zero remove the space on the sides of the division tags**/
body
{
  margin: 0;
  padding: 0;
}
h1, h4
{
  font-family: 'Montserrat', serif;
}

.header
{
  color: white;
  margin-top: 15%;
  margin-left: 5%;
  margin-bottom: 30%;
  font-size: 150%;
}

/**Add in the background image**/
.parallax
{
  display: block;
  overflow: hidden;
  background-image: url("images/background1.jpg");
  width: 100%;
  height: auto;
  background-attachment: fixed; /**Fixing the background prevents it from scrolling with the rest of the page**/
  background-repeat: no-repeat;
  background-size: cover;
}
```

Save the file and refresh the website. It should show the parallax scrolling effect.

#### Step 5: Styling the Foreground Container

```
/**Styling the foreground container**/
.foreground-container
{
  padding-bottom: 20%;
}
.head-sample
{
  margin-top: 10%;
  text-align: center;
  font-size: 250%;
}
.table1
{
  width: 80%;
  padding-top: 5%;

}
.table1 td
{
  display: absolute;
  position: relative;
  text-align: center;
  padding: 0%;

}
```

We will add an image overlay to the featured image links.

```
/*Overlay*/
.overlay
{
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background: rgba(0,0,0,0.5);
}

.feature:hover .overlay
{
  opacity: 1;
}

.text
{
  position: absolute;
  color: white;
  font-family: 'Montserrat';
  font-size: 250%;
  top: 45%;
  left: 35%;
}
```

#### Step 6: Adding style and parallax scrolling to Ending Container

```
.ending
{
  display: inline-block;
  background: rgba(0, 0, 0, 0.5);
  color: white;
  font-size: 150%;
  height: 100%;
  width: 100%;
  top: 50%;
  padding-top: 24%;
  padding-bottom: 15%;

}

.parallax2
{
  display: block;
  overflow: hidden;
  background-image:url("images/background2.jpg");
  width: 100%;
  height: auto;
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
}

```

Save the file and refresh the website.
