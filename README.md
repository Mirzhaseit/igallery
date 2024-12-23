# Ex.08 Design of Interactive Image Gallery
## Date:23/12/24

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Faces Behind the Music</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #faf6f8;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh; 
            margin: 0;
            flex-direction: column;
        }

        .gallery-container {
            text-align: center;
            width: 100%;
        }

        h1 {
            font-size: 30px;
            color: #181919;
            margin-bottom: 20px;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px; 
        }

        .gallery-item {
            width: 250px; 
            height: 250px;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .gallery-item:hover {
            transform: scale(1.5);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            z-index: 1;
        }

        footer {
            text-align: center;
            font-size: 16px;
            margin-top: 20px; 
            color: #333;
        }
    </style>
</head>
<body>
    <div class="gallery-container">
        <h1>The Faces Behind the Music</h1>
        <div class="gallery">
            <div class="gallery-item"><img src="aniruth.png" alt="Singer 1"></div>
            <div class="gallery-item"><img src="AR.png" alt="Singer 2"></div>
            <div class="gallery-item"><img src="gv.png" alt="Singer 3"></div>
            <div class="gallery-item"><img src="karthik.png" alt="Singer 4"></div>
            <div class="gallery-item"><img src="sain.png" alt="Singer 5"></div>
            <div class="gallery-item"><img src="sg.png" alt="Singer 6"></div>
            <div class="gallery-item"><img src="swetha.png" alt="Singer 7"></div>
            <div class="gallery-item"><img src="jonita.png" alt="Singer 8"></div>
        </div>
    </div>
    <footer>
        Designed and developed by MIRZHA FATHIMA S; 2024
    </footer>

    <script>
        function zoomInOut(imageId) {
            var image = document.getElementById(imageId);
            if (image.style.transform === "scale(2)") {
                image.style.transform = "scale(1)";  
            } else {
                image.style.transform = "scale(2)";  
            }
        }
    </script>
</body>
</html>

```

## OUTPUT:

![alt text](gallery.png)
![alt text](gal2.png)



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
