# Ex.06 Book Front Cover Page Design
## Date: 29-09-2024

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
	<title>Photo Gallery</title>
	<link rel="stylesheet" href="css/gallery.css">
	<script src = "js/gallery.js"></script>
</head>
<body>
	
	<div id = "image">
		Hover over an image below to display here.
	</div>
	
	<img class = "preview" alt = "Styling with a Bandana" src = "https://s3-us-west-2.amazonaws.com/s.cdpn.io/389177/bacon.jpg" onmouseover = "upDate(this)" onmouseout = "unDo()">
	
	<img class = "preview" alt = "With My Boy" src = "https://s3-us-west-2.amazonaws.com/s.cdpn.io/389177/bacon2.JPG" onmouseover = "upDate(this)" onmouseout = "unDo()">
	
	<img class = "preview" src = "https://s3-us-west-2.amazonaws.com/s.cdpn.io/389177/bacon3.jpg" alt = "Young Puppy" onmouseover = "upDate(this)" onmouseout = "unDo()">

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
## WEBSITE LINK
```
https://codepen.io/Harish_-Ammu/pen/WNVQGOw
```
## OUTPUT:

![Screenshot 2024-09-29 182707](https://github.com/user-attachments/assets/c2941879-c36a-49fd-b5eb-d3187cbe80fc)

![Screenshot 2024-09-29 182641](https://github.com/user-attachments/assets/8bc9c8e2-b672-403b-b4cd-3733b1182ac4)

![Screenshot 2024-09-29 182652](https://github.com/user-attachments/assets/6d3783d2-6a3d-4fd2-9ca3-0f28ab8a8916)

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
