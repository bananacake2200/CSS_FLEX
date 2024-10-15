#CSS_FLEX

## CSS Flexbox (Flexible Box Layout) 
Is a layout model in CSS designed to efficiently arrange items within a container, even when their size is dynamic or unknown. It allows you to control the alignment, spacing, and distribution of items along both the main axis (horizontal or vertical) and the cross axis. This makes Flexbox especially useful for building responsive web layouts.

## Key Concepts in Flexbox:
* Flex Container: The parent element that holds flex items. You define it by setting display: flex; or display: inline-flex; on the container.

* Flex Items: The direct children of a flex container. These items are laid out along a main axis and a cross axis.

## Common Properties:
### flex-direction: Defines the direction in which flex items are laid out. Options include:

* row (default): Items are laid out horizontally.
* column: Items are laid out vertically.
* row-reverse or column-reverse: Reverses the direction.

### justify-content: Aligns flex items along the main axis. Common values:

* flex-start: Items start from the beginning of the container.
* center: Items are centered.
* space-between: Items are evenly spaced with the first and last item at the edges.
* space-around or space-evenly: Adds space around items.

### align-items: Aligns flex items along the cross axis. Common values:

* flex-start, center, flex-end, stretch.

### flex-wrap: Controls whether flex items should wrap onto multiple lines when they overflow the container.

* nowrap (default): No wrapping.
* wrap: Wrap items onto new lines.

### flex-grow, flex-shrink, flex-basis: These define how flex items grow, shrink, and set their initial size in relation to others.


##

## Sample Output

## styles.css
```css
/* default styles */
body, h1, h2, p {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f8f9fa;
    color: #333;
    background-image: url(kuromi-hello-kitty-3840x2160-9495.png);
    background-repeat: no-repeat;
}

/* Login section */
.login-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 40px;
    border-radius: 5px;
    border: 1px solid black;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    margin: 5% auto;
    width: 300px; 
    height: 300px;
    backdrop-filter: blur(5px);
}

.login-form {
    display: flex;
    flex-direction: column; 
    width: 100%;
}

label {
    margin: 10px 0 5px;  
}

input, textarea {
    width: 100%;
    padding: 10px;
    border: 1px #000000;
    border-radius: 5px;
    margin: 5px 0 10px 0;
}

button {
    padding: 10px 50px;
    background-color: #0e0f0f;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
    margin-top: 15px;
}

button:hover {
    background-color: #d49dd7;
    color: black;
}

/* Header */
header {
    background-color: #201b20; 
    color: rgb(237, 228, 228);
    padding: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

h1 {
    margin-bottom: 10px;
}

.nav-list {
    display: flex;
    justify-content: space-around;
    list-style-type: none;
    padding: 0;
    width: 100%;
}

.nav-list li a {
    color: rgb(255, 255, 255);
    text-decoration: none;
    padding: 10px 15px;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

.nav-list li a:hover {
    background-color: #0056b3;  
}

/* Product page */
.products {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 20px;
}

.product-card {
    flex: 1 1 30%;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 20px;
    padding: 15px;
    background-color: white;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card:hover {
    transform: scale(1.05);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

/* About page */
.about-section {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #fff;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    max-width: 700px;
    margin: 5%;
    margin-left: 25%;
}

.about-content {
    text-align: center;
}

h2 {
    font-size: 1.3rem;
    color: #333;
    margin-bottom: 20px;
}

p {
    font-size: 1.1rem;
    line-height: 1.6;
    color: #555;
    margin-bottom: 15px;
}

/* Contact page */

.form-section {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    margin-top: 5%;
}

.contact-form {
    display: flex;
    flex-direction: column;
    background-color: #fff;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    max-width: 400px;
    width: 100%;
}

.contact-form label {
    margin-bottom: 8px;
    font-weight: bold;
}

.contact-form input, 
.contact-form textarea {
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 1rem;
}

/* Form */
.form {
    position: relative;
    width: 740px;
    height: 400px;
    background: linear-gradient(to right, #faf8fa, #c19ccc);
    border: 2px solid rgba(8, 8, 8, 0.5);
    border-radius: 20px;
    backdrop-filter: blur(15px);
    display: flex;
    justify-content: center;
    align-items: center;
}
.employee-cards {
    display: flex;
    justify-content: space-around;
    padding: 20px;
}

/* Employee card */

.employee-card {
    flex: 1;
    margin: 10px;
    padding: 20px;
    border: 1px solid #000000;
    border-radius: 5px;
    text-align: center;
    background-color: white;
}

.employee{
margin: 3%;
padding-left: 40%;
font-size: 2rem;
}
```

## index.html

![homepage](https://github.com/user-attachments/assets/c7f142b3-66ed-47a3-8169-bae49fefa5be)

##

## product.html

![product](https://github.com/user-attachments/assets/1f308fea-e5ea-4064-8966-b2a759bfd20e)

## contact.html

![contact](https://github.com/user-attachments/assets/fe33afb1-17f5-48f8-ae96-1c263bb5e0ce)

##

## about.html

![about](https://github.com/user-attachments/assets/b75416b8-a0ab-4998-95d3-18750b283a7b)

##

## employee.html

![employee](https://github.com/user-attachments/assets/1105583c-50f0-4b2f-aaa0-4a8040efb778)

##
