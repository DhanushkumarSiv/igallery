# Ex.08 Design of Interactive Image Gallery
## Date:18/12/2024

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
image.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Bebas+Neue&family=Edu+AU+VIC+WA+NT+Arrows:wght@400..700&family=Josefin+Sans:ital,wght@0,100..700;1,100..700&family=Montserrat:ital,wght@0,100..900;1,100..900&family=Raleway:ital,wght@0,100..900;1,100..900&family=Shadows+Into+Light&display=swap" rel="stylesheet">
</head>
<body>
    <div class="first">
    <h1 class="heading">
        Interactive Image Gallery 🖼️
    </h1>
    </div>
    <div>
        <center>
        <img src="leo.jpg" class="img">
        <h3>LEO</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="sarkar.jpg" class="img">
        <h3>SARKAR</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="gilli.jpg" class="img">
        <h3>GHILLI</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="pokkiri.jpg" class="img">
        <h3>POKKIRI</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="kaththi.jpg" class="img">
        <h3>KATHTHI</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="master.jpg" class="img">
        <h3>MASTER</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="beast (2).jpg" class="img">
        <h3>BEAST</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="bigil.jpg" class="img">
        <h3>BIGIL</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="politician (2).jpg" class="img">
        <h3>POLITICIAN</h3>
        </center>
    </div>
    <div class="action">
        <img src="" alt="" class="action-image">
        <button class="btn">X</button>
    </div>
    <footer>
        Designed and Developed by DHANUSH &reg;
    </footer>
    <script>
        const action = document.querySelector('.action');
        const actionImage = document.querySelector('.action-image');
        const closeButton = document.querySelector('.btn');
        const images = document.querySelectorAll('.img');

        images.forEach((image) => {
            image.addEventListener('click', () => {
                actionImage.src = image.src;
                action.classList.add('visible'); 
            });
        });

        closeButton.addEventListener('click', () => {
            action.classList.remove('visible'); 
        });

       action.addEventListener('click', (e) => {
            if (e.target === action) {
                action.classList.remove('visible'); 
            }
        });
    </script>
</body>
</html>

style.css

.heading{
    text-align: center;
    font-size: 30px;
    font-family: Montserrat;
    color: rgb(83, 42, 42);

}
.first {
    background-image: linear-gradient(to left,#eeaeca,);
    color:red;
    height:80px;
    width: 1461px;
    padding: 25px;
}
div{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    display: inline-block;
    margin: 25px;

}
div img{
    width: 420px;
    height: 350px;
    border:2px solid;
    border-radius: 13px;
    box-shadow: 4px 7px 7px 0px;
    margin:10px;
    transition: 400ms;

}
.img:hover {
    transform: scale(1.05); 
}

.action {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    background-color: rgba(0, 0, 0, 0.8);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
    visibility: hidden;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.action.visible {
    
    visibility: visible;
    opacity: 1;
}

.action-image {
    max-width: 90%;
    max-height: 90%;
    border-radius: 10px;
}

.btn {
    position: absolute;
    top: 10px;
    right: 10px;
    padding: 10px 20px;
    font-size: 16px;
    color: #fff;
    background: rgba(0, 0, 0, 0.5);
    border: none;
    cursor: pointer;
    border-radius: 5px;
    transition: background 0.2s ease;
}

.btn:hover {
    background: rgba(255, 255, 255, 0.2);
}
body{
    background-image: url(pexels-pixabay-235985.jpg);

}
footer{
    height:55px;
    width: 1600px;background-color: rgb(90, 42, 42);
    text-align: center;
    padding-top: 30px;
    font-size: large;
    font-family: Montserrat;
    color:white ;    
}


```

## OUTPUT:
![alt text](55.png)

![alt text](56.png)

![alt text](57.png)

![alt text](58.png)

![alt text](59.png)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
