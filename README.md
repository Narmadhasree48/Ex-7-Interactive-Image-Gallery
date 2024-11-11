# Ex-7-Interactive-Image-Gallery
## Date: 11-11-2024

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

### index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Photo Gallery</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <h1>Interactive Photo Gallery</h1>
  <div id="image">Hover over an image below to display here.</div>

  <div class="gallery">
    <img class="preview" alt="beauty of nauture" src="https://images.pexels.com/photos/16373111/pexels-photo-16373111/free-photo-of-sunlight-over-dirt-road-in-forest-in-winter.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="sunlight" src="https://images.pexels.com/photos/1420440/pexels-photo-1420440.jpeg?auto=compress&cs=tinysrgb&w=600" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" src="https://images.pexels.com/photos/2295744/pexels-photo-2295744.jpeg?auto=compress&cs=tinysrgb&w=600" alt="wildlife" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="Mountain" src="https://images.pexels.com/photos/1743165/pexels-photo-1743165.jpeg?auto=compress&cs=tinysrgb&w=600" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="night snow" src="https://images.pexels.com/photos/10620135/pexels-photo-10620135.jpeg?auto=compress&cs=tinysrgb&w=600" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" src="https://images.pexels.com/photos/77171/pexels-photo-77171.jpeg?auto=compress&cs=tinysrgb&w=600" alt="london" onmouseover="upDate(this)" onmouseout="unDo()">
  </div>
  <script src="script.js"></script>
</body>

</html>
```

### gallery.css
```
body{
    margin: 2%;
    border: 1px solid black;
    background-color: #b3b3b3;
}
#image{
line-height:650px;
    width: 575px;
height: 650px;
    border:5px solid black;
    margin:0 auto;
background-color: #8e68ff;
background-image: url('');
background-repeat: no-repeat;
color:#FFFFFF;
text-align: center;
background-size: 100%;
margin-bottom:25px;
font-size: 150%;
}
.preview{
    width:10%;
    margin-left:17%;
border: 10px solid black;
}
img{
    width:95%;
}

```
### gallery.js
```
// Reference to the image container
const imageDiv = document.getElementById('image');
const originalImageUrl = ''; // Set this to the URL of your original image
const originalText = "Hover over an image below to display here."; // Original text

function upDate(previewPic) {
    // Change the background image to the source of the hovered image
    imageDiv.style.backgroundImage = `url('${previewPic.src}')`;
    
    // Update the text to the alt text of the hovered image
    imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
    // Reset the background image to the original URL
    imageDiv.style.backgroundImage = `url('${originalImageUrl}')`; // Use the original image URL here
    
    // Change the text back to the original text
    imageDiv.innerHTML = originalText;
}
```
## WEBSITE URL
https://codepen.io/narmadha-s/pen/OJKrQdP
## OUTPUT:
![Screenshot (37)](https://github.com/user-attachments/assets/c5fd283b-794d-4033-97eb-7f6fc3e33d2a)

![Screenshot (38)](https://github.com/user-attachments/assets/7a2f92d2-c150-4e84-b5b2-3bb06fd22149)


## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
