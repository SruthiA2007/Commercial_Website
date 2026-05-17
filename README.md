# Ex02 Commercial Website
## Date: 17/05/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PosterVerse | Home</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <div class="logo">PosterVerse</div>
    <nav>
        <a href="index.html">Home</a>
        <a href="products.html">Posters</a>
        <a href="contact.html">Contact</a>
    </nav>
</header>

<section class="hero">
    <div class="hero-content">
        <h1>Decorate Your World</h1>
        <p>Premium Wall Posters for Every Space</p>
        <a href="products.html" class="btn">Shop Now</a>
    </div>
</section>

<footer>
    <p>© 2026 PosterVerse | All Rights Reserved</p>
</footer>

</body>
</html>
```
product.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PosterVerse | Products</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <div class="logo">PosterVerse</div>
    <nav>
        <a href="index.html">Home</a>
        <a href="product.html">Posters</a>
        <a href="contact.html">Contact</a>
    </nav>
</header>

<section class="products-section">
    <h2>Our Poster Collection</h2>

    <div class="product-container">

        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1541963463532-d68292c34b19?auto=format&fit=crop&w=800&q=80" alt="Nature Poster">
            <h3>Nature Landscape</h3>
            <p>₹899</p>
            <button>Buy Now</button>
        </div>

        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=800&q=80" alt="Abstract Poster">
            <h3>Abstract Art</h3>
            <p>₹1,199</p>
            <button>Buy Now</button>
        </div>

        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1492724441997-5dc865305da7?auto=format&fit=crop&w=800&q=80" alt="City Poster">
            <h3>City Skyline</h3>
            <p>₹999</p>
            <button>Buy Now</button>
        </div>

        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1501594907352-04cda38ebc29?auto=format&fit=crop&w=800&q=80" alt="Quote Poster">
            <h3>Motivational Quote</h3>
            <p>₹799</p>
            <button>Buy Now</button>
        </div>

    </div>
</section>

<footer>
    <p>© 2026 PosterVerse | All Rights Reserved</p>
</footer>

</body>
</html>
```
contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PosterVerse | Contact</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <div class="logo">PosterVerse</div>
    <nav>
        <a href="index.html">Home</a>
        <a href="products.html">Posters</a>
        <a href="contact.html">Contact</a>
    </nav>
</header>

<section class="contact-section">
    <h2>Contact Us</h2>

    <div class="contact-container">

        <div class="contact-info">
            <p><strong>Email:</strong> support@posterverse.com</p>
            <p><strong>Phone:</strong> +91 9876543210</p>
            <p><strong>Address:</strong> 101 Creative Street, Delhi, India</p>
        </div>

        <div class="contact-form">
            <input type="text" placeholder="Your Name">
            <input type="email" placeholder="Your Email">
            <textarea rows="4" placeholder="Your Message"></textarea>
            <button>Send Message</button>
        </div>

    </div>
</section>

<footer>
    <p>© 2026 PosterVerse | All Rights Reserved</p>
</footer>

</body>
</html>
```
style.css
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background: #f4f4f4;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 8%;
    background: #111;
    color: white;
}

nav {
    display: flex;
    gap: 25px;
}

nav a {
    text-decoration: none;
    color: white;
    transition: 0.3s;
}

nav a:hover {
    color: orange;
}

.hero {
    height: 75vh;
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
                url("https://images.unsplash.com/photo-1519681393784-d120267933ba?auto=format&fit=crop&w=1400&q=80");
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
}

.btn {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    background: orange;
    color: white;
    text-decoration: none;
}

.products-section {
    padding: 60px 8%;
    text-align: center;
    background: #ffffff;
}

.product-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 30px;
    margin-top: 30px;
}

.product-card {
    width: 250px;
    background: white;
    border-radius: 8px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
    overflow: hidden;
    transition: 0.3s;
}

.product-card:hover {
    transform: translateY(-10px);
}

.product-card img {
    width: 100%;
    height: 300px;
    object-fit: cover;
}

.product-card h3 {
    margin: 10px 0;
}

.product-card button {
    margin: 10px;
    padding: 8px 20px;
    border: none;
    background: #111;
    color: white;
    cursor: pointer;
}

.product-card button:hover {
    background: orange;
}

.contact-section {
    padding: 60px 8%;
    background: #222;
    color: white;
}

.contact-container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 40px;
    margin-top: 30px;
}

.contact-form {
    display: flex;
    flex-direction: column;
    flex: 1;
}

.contact-form input,
.contact-form textarea {
    margin-bottom: 15px;
    padding: 10px;
    border: none;
}

.contact-form button {
    padding: 10px;
    border: none;
    background: orange;
    color: white;
    cursor: pointer;
}

footer {
    background: #111;
    color: white;
    text-align: center;
    padding: 20px;
}

```
## OUTPUT
<img width="1238" height="668" alt="image" src="https://github.com/user-attachments/assets/ff1f6db2-ae2f-417d-821c-0eaa186048d3" />

<img width="1228" height="707" alt="image" src="https://github.com/user-attachments/assets/3870b475-f083-42e8-9dc7-9e94c91c56f3" />

<img width="1242" height="636" alt="image" src="https://github.com/user-attachments/assets/810eccf0-c75d-45fa-a026-616ecb80abbe" />



## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
