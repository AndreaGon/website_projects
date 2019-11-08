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

#### Step 2 (HTML): Adding the Head

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

-```<title></title>```: Displays the title of the web page in the title bar.
- ```<meta charset="utf-8"/>```: It specifies how each character will be encoded.

Save the file as ```index.html```.


#### Step 3 (HTML): Adding the Body

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
