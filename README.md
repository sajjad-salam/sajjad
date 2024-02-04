 ### Project: Personal Portfolio Website with Blurred Background Animation

**Introduction:**
This project aims to create a visually appealing personal portfolio website that showcases a user's profile, including their social media links, contact information, and a brief introduction. The website features a blurred background animation using CSS and SVG shapes to enhance the overall design.

**Step 1: HTML Structure**
The HTML structure consists of a basic layout with a container for the profile card and a blurred background container. The profile card includes sections for the user's profile image, name, social media icons, and a brief description.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Sajjad Salam </title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div class="blur-container">
            <div class="shape"></div>
            <div class="shape" style="--offset:180deg; --speed: 6000ms; --background: linear-gradient(cyan, blue, green, purple, cyan);"></div>
        </div>
        <div class="card">
            <!-- Profile details go here -->
        </div>
    </div>
</body>
</html>
```

**Step 2: CSS Styling**
The CSS stylesheet defines the layout, typography, and visual appearance of the website. It includes styles for the profile card, blurred background animation, and social media icons.

```css
/* Blurred background and shapes styles */
.blur-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 1;
    overflow: hidden;
}

.shape {
    margin: 0 auto;
    aspect-ratio: 1;
    position: relative;
    --width: 100%;
    --scale: 1;
    --opacity: 0.66;
    --top: 0;
    --left: 

