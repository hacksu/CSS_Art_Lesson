# Getting Started with CSS Art!

# Cloning this GiHub Repo
To start this lesson, you will need to fork this repo by clicking on the button on the right hand side of the screen that says "fork" This will take a few moments.
Then, once the forking is complete, clone your forked repo in order to have the base code required for the lesson.
Cloning is done with the following steps:
  1. Check that you have git
        If you are unsure what I am talking about, please ask! We would love to help you set it up :)
  2. Navigate with command line to a folder that you would like to place the file
  3. Click on the button that says clone and copy the url
  4. Type in the following command to do so:
```
git clone repo [paste url here]
```
You have cloned successfully!

# What Code Do We Have
The following code is what you have to start off with 
```
<body>
    <head>
        <link rel="stylesheet" type="text/css" href="cssArt.css">
    </head>
  
    <div class = "Box">
        <!-- Circular Head -->
        <div class = "Head">
         <!-- Circular Head Copy -->
        <div class = "Head-copy"></div>
    
        <!--Left Ear  -->
        <div class = "Left-ear">
            <!--Inner Ear -->
            <div class ="Inner-ear"></div>
        </div>
            
        <!--Right Ear -->
        <div class = "Right-ear">
            <!--Inner Ear -->
            <div class ="Inner-ear"></div>
        </div>
    
        <!-- Left Outer Eye -->
        <div class = "Eye-left">
            <!--Pupil-->
            <div class = "Pupil">
                <div class = "otherPupil">
                </div>
                </div>
        </div>
    
        <!-- Right Outer Eye  -->
        <div class = "Eye-right">
            <!--Pupil-->
            <div class = "Pupil">
                <div class = "otherPupil">
                </div>
                </div>
        </div>
    
        <!-- Nose  -->
        <div class = "Nose"></div>
        <!-- End Head-->
    </div>
</body>
```
Each part of the above code is a different part of the animal. What animal is it? That is for you to figure out with the code :)
Each div is a different part of the animal. Think of the code as if you are drawing a picture. You are meant to start with the background and work your way forward. 


# Code We are Going to Add: Code Time! :)
All the code we are going to is purely CSS. Each element of the css is what shapes the divs to form the art that we are trying to complete. 
Here is what we have 
```
body{
  background: white;
}

.Box{
}

.Head{
}

.Head-copy{
}

.Left-ear{
}

.Right-ear{
}

.Inner-ear{
}

.Eye-left{
}

.Eye-right{
}

.Pupil{
}

.Nose{
}

.otherPupil{
}
```
As you can see nothing is styled! So this is where we start adding style elements to form the image.
For all of the divs, we are going to change their shape, position, and color.
Shape is adjusted by margin and radius of the div, while color is set with either a hex value or a keyword such as blue. Lastly, position is adjusted with margin, height, width, z-index, and position. Z-index is how far away the div is from the canvas. This is important when having to place divs behind other divs to get a better looking image. Position can be set to may different keywords.
  1. Relative
  2. Absolute
  3. Sticky
  4. Static
  5. Fixed 
For our lesson, we are only going to focus on relative and absolute. Relative is positioned relative to its normal position, and absolute places divs relative to its closest ancester.

First we are going to start with the box. Think of this as the canvas for you to start painting on. Everything we code is to be housed in this box. This box is going to be relative in position.

```
.Box{
  position: relative;
  margin: auto;
  display: block;
  margin-top: 8%;
  width: 600px;
  height: 420px;
  background: #C000F5;
}
```

Next we are going to copy the heads, and yes, I said heads. There are two heads because one is on another part of the plane. The head copy is raised above the other to allow for elements to be sandwiched inbetween the two divs.
```
.Head{
  position: absolute;
  top: 16.5%;
  left: 25%;
  width: 50%;
  height: 67%;
  background: #A6BECF;
  border-radius: 50%;
}

.Head-copy{
  width: 100%;
  height: 100%;
  position: absolute;
  background: #924D3B;
  border-radius: 50%;
  z-index: 2;
}
```
Then we are going to add ears behind the head copy, and add inner ear for depth.
```
.Left-ear{
  position: absolute;
  left: 15%;
  top: -10%;
  border-left: 50px solid transparent;
  border-right: 50px solid transparent;
  border-bottom: 100px solid #924D3B;
  border-radius: 50%;
}

.Right-ear{
  position: absolute;
  border-left: 50px solid transparent;
  border-right: 50px solid transparent;
  border-bottom: 100px solid #924D3B;
  right: 15%;
  top: -10%;
  border-radius: 50%;
}

.Inner-ear{
  position: absolute;
  border-radius: 50%;
  width: 80%;
  height: 80%;
  top: 10%;
  left: 10%;
  background: #819CAF;
}
```
Once the ears are completed, we are going to add the eyes and the pupils.
```

.Nose{
    position: absolute;
    border-left: 50px solid transparent;
    border-right: 50px solid transparent;
    border-top: 100px solid blue;
    left: 34.5%;
    top: 57.5%;
    border-radius: 50px;
    z-index: 4;
  }
```
What animal do you see? Is it an owl! You bet!
