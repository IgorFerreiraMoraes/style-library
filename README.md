# style-library

My own web styles library (See in https://igorferreiramoraes.github.io/style-library/).
It is composed of 2 main colors and the text color of each, that can be changed in:
:root{
    --mainColor: hsl(204, 70%, 53%);
    --mainTextColor: hsl(204, 71%, 81%);

    --secondColor:  hsl(324, 70%, 53%);
    --secondTextColor: hsl(324, 71%, 81%);
}

--

Boxes:
There are 4 boxes
The White One, <div class="box">
The Black One, <div class="box black">
The Main Box, <div class="box main">
The Secondary Box, <div class="box second">

The Main and Secondary boxes' colors are the Main and Secondary colors defined in the root.

--

Images:

Hover <div class="hover">
Needs a background-image
When the user puts the mouse on the image, the image is zoomed
We can put a div inside the hover
<div class="hover"> <div>Txt Inside the hover</div></div>
The content of the inside div is then showed when the user puts the mouse on the image

Paralax <div class="paralax">
Needs a background-image
The image is fixed

Text & Image
Text with a color in the left and the image is in the right
<div class="text-img second">
	<p>The text to appear</p>
	<div style="background-image:url(image to appear);"></div>
</div>
We can change the background of the text to the main or secondary colors by using
<div class="text-img main"> or <div class="text-img second">

Cards 
Image with a text description bellow
<div class="card">
	<img src="the image to appear">
                <div>
                    The text to Appear
                </div>
</div>
We can change the background of the text to black,main or secondary colors by using
 <div class="card black">,  <div class="card main"> or  <div class="card second">

Slideshow
We need a <div class="slide-container" style="width: 60%;"></div> to create the slideshow
inside of the container, we are adding slides
<div class="slide">
                <div class="slide-number">Number of slide</div>
                <img src="the image"">
                <div class="slide-text">Caption Text</div>
</div>

then, we need the buttons to navigate the slides
<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

also, a way to select the slides
<button onclick="currentSlide(numberOfSlide)">go to certain slide</button>

--

Buttons:
We have 3 types of buttons

<button class="btSlide"></button>
<button class="btFill">This one can have the class "right"</button>
<button class="btRound"></button>

all three can have the classes "second" or "black" in order to change the background

--

Drop Downs:

Drop Image
<div class="dropImg">
            <img src="your image">
            <div>
                things to appear when hovered
            </div>
</div>

Drop Button
<div class="dropdown">
            <button class="btFill">Hover Me</button>
            <div class="dropdown-content">
                <a href="#">Link 1</a>
                <a href="#" class="second">Link 2</a> 
                <a href="#">Link 3</a>
            </div>
</div>

Drop Text
<div class="detail">
            <h2 class="detail-title">Title, click to show more</h2>
            <div class="detail-content">
                Content to appear
            </div>
</div>


 
