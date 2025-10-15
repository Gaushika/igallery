# Ex.08 Design of Interactive Image Gallery
## Date:13/10/2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
photo.html
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Multiple Images Enlarge on Click</title>
  <link rel="stylesheet" href="style.css">

</head>
<body>

<h1 align="center"  >Gaushika RR (25017292)</h1>
  <div class="image-container">
    <img class="clickable-image" src="i1.png" alt="Image 1" />
    <img class="clickable-image" src="i2.png" alt="Image 2" />
    <img class="clickable-image" src="i3.png" alt="Image 3" />
    <img class="clickable-image" src="i4.png" alt="Image 4" />
  </div>

  <script>
    const images = document.querySelectorAll('.clickable-image');

    images.forEach(img => {
      img.addEventListener('click', () => {
        img.classList.toggle('enlarged');
      });
    });
  </script>

</body>
</html>



style.css

*{
    background-color: rgb(243, 117, 155);
}
.image-container {
  display: flex;
  justify-content: center; 
  align-items: center;     
  gap: 10px;              
  padding: 20px 0;
}

.clickable-image {
  width: 150px;
  height: auto;
  cursor: pointer;
  transition: transform 0.3s ease;
  position: relative;
  flex-shrink: 0;
.image-container {
  gap: 10px;
  padding: 20px 0;
  justify-content: center; 
}

.clickable-image {
  width: 150px;
  height: auto;
  cursor: pointer;
  transition: transform 0.3s ease;
  position: relative;
  flex-shrink: 0;
}

.clickable-image:hover {
  transform: scale(1.2);
  z-index: 5;
}

.clickable-image.enlarged {
  transform: scale(2);
  z-index: 10;
}
}

.clickable-image:hover {
  transform: scale(1.2);
  z-index: 5;
}

.clickable-image.enlarged {
  transform: scale(2);
  z-index: 10;
}


```
## OUTPUT:
![alt text](<Screenshot (49).png>)
![alt text](<Screenshot (50).png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
