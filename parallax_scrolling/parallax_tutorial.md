# Parallax Scrolling Effect Using HTML & CSS


### Overview
A parallax scrolling is a type of web design where the background content moves at a different speed than the foreground content as the user scrolls.

##### Website without Parallax Scrolling Effect
https://www.w3schools.com/howto/tryhow_css_parallax_demo_none.htm

##### Website with Parallax Scrolling Effect
https://www.w3schools.com/howto/tryhow_css_parallax_demo.htm


### When To Use Parallax Scrolling?
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
  </head>
</html>
```
What does this mean?
- ```<!DOCTYPE html>```: It tells the web browser what version of HTML we are using. Currently, we are using HTML 5
- ```<html></html>```: It is where all the HTML elements are contained.
- ```<head></head>```: The head tag is the container for the head elements. Head elements include the title, the linked style, the meta information, and more.
- ```<title></title>```: Displays the title of the web page in the title bar.
- ```<meta charset="utf-8"/>```: It specifies how each character will be encoded.

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

This will be the background content. Currently, it doesn't have background image. It only contains the headers.

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

#### Step 4: Adding the CSS

Create a new file and name it as main.css. Save it in the same folder with the index.html file.





