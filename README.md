# Web Design for a Software Product Company

## AIM:

To design a static website for a software product company company.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Updating the sample content.

### Step 4:

Choose the appropriate style and color scheme.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
### Home.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Ferrari</title>
  <style>
    body {
  font-family: Arial, sans-serif;
  margin: 650px;
  background-image: url(pexels-mike-bird-5759866.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}



    .overlay {
      background-color: rgba(0, 0, 0, 0.7);
      padding: 20px;
      border-radius: 10px;
      color: #ffffff;
      position: absolute;
      top: 90%;
      left: 50%;
      transform: translate(-50%, -50%);
    }

    h1 {
      color: #dc3545;
    }

    p {
      line-height: 1.5;
    }

    footer {
      text-align: center;
      color: #ffffff;
      margin-top: 40px;
    }
  </style>
</head>
<body>
    <header>
        <div class="menu-icon" onclick="document.querySelector('.menu').classList.toggle('open')">
          <div class="menu-line"></div>
          <div class="menu-line"></div>
          <div class="menu-line"></div>
          <span color="white">Menu</span>
        </div>
        <div class="menu">
          <ul>
            <li><a href="fabout.html">ABOUT</a></li>
            <li><a href="polo-shirt.html">Featured Cars</a></li>
            
          </ul>
        </div>
      </header>
  <div class="overlay">
    
    <h1>About Ferrari</h1>
  
    <img src="ferrari-logo.png" alt="Ferrari Logo" width="200">

    <p>Ferrari is an Italian luxury sports car manufacturer based in Maranello, Italy. The company was founded in 1939 by Enzo Ferrari as Auto Avio Costruzioni, and later officially became Ferrari S.p.A. in 1947.</p>

    <p>Ferrari is renowned for producing high-performance sports cars, iconic racing vehicles, and luxury grand tourers. The brand's vehicles are known for their powerful engines, exquisite design, and cutting-edge technology.</p>

    <p>Over the years, Ferrari has achieved great success in motorsport, particularly in Formula One racing. The team has won numerous championships and has been home to legendary drivers such as Michael Schumacher and Niki Lauda.</p>

    <p>Today, Ferrari continues to create some of the most coveted and sought-after cars in the world. Their lineup includes models such as the 488 GTB, 812 Superfast, and SF90 Stradale, among others.</p>

    <p>Aside from their road cars, Ferrari also produces limited-edition models and special series vehicles that exemplify exclusivity and performance. These limited-production cars often become highly collectible and are cherished by automotive enthusiasts worldwide.</p>

    <p>With a rich heritage, a commitment to innovation, and a dedication to excellence, Ferrari remains a symbol of automotive excellence and a dream for many passionate drivers and enthusiasts.</p>

    <footer>
      &copy; 2023 Ferrari. All rights reserved.
    </footer>
  </div>
  <footer>
    &copy; 2023 Ferrari. All rights reserved.
  </footer>
</body>
</html>

```
### index.html
```
<!DOCTYPE html>
<html>
<head>
  <title>FERRARI</title>
  <link rel="stylesheet" type="text/css" href="fstyle.css">
  <style>
    /* Add your custom styles here */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      height: 100px;
      background-color: #ffffff;
    }
  
    /* Add your custom styles here */
  
    .banner {
      margin: 0;
      padding: 0;
      background-image: linear-gradient(to top right, rgba(228,221,221, 0.50) 20%, rgba(0,0,0, 0.60 ) 25%), url(ferrari_banner.jpg);
      background-position: top;
      background-size: cover;
      background-repeat: no-repeat;
      height: 800px;
      display: flex;
      align-items: center;
      justify-content: center;
    }
  
    .banner-button {
      font-size: 18px;
      background-color: #ff5c5c;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 4px;
      cursor: pointer;
      text-transform: uppercase;
      transition: background-color 0.3s ease;
    }
  
    .banner-button:hover {
      background-color: #ff4242;
    }
  
    main {
      padding: 40px;
    }
  
    section {
      margin-bottom: 40px;
    }
  
    h2 {
      font-size: 32px;
      margin-bottom: 20px;
    }
  
    .product-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-gap: 20px;
    }
  
    .product {
      text-align: center;
    }
  
    .product img {
      width: 100%;
      max-height: 200px;
      object-fit: cover;
      border-radius: 4px;
      margin-bottom: 10px;
    }
  
    .person-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-gap: 20px;
    }
  
    .person {
      text-align: center;
    }
  
    .person img {
      width: 50%;
      max-height: 350px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 50px;
    }
  
    address {
      font-style: normal;
      margin-bottom: 10px;
    }
  
    footer {
      background-color: #333;
      color: #fff;
      padding: 20px;
      text-align: center;
    }

    /* Menu styles */
    .menu-icon {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      width: 70px;
      height: 100px;
      cursor: pointer;
      position: absolute;
      top: 0px;
      left: 20px;
      z-index: 9999;
      color: white;
    }
  
    .menu-line {
      width: 70%;
      height: 5px;
      background-color: #a04020;
      margin-bottom: 4px;
    }
  
    .menu {
      display: none;
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(49, 46, 46, 0.8);
      z-index: 999;
    }
  
    .menu.open {
      display: block;
    }
  
    .menu ul {
      list-style: none;
      padding: 0;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  
    .menu ul li {
      margin-bottom: 10px;
    }
  
    .menu ul li a {
      text-decoration: none;
      color: #fff;
    }

    .footer-column {
      text-align: center;
    }

    .footer-content {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }

    .social-media-list {
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top: 10px;
    }

    .social-media-list li {
      margin-right: 10px;
    }

    .social-media-list li:last-child {
      margin-right: 0;
    }

    .social-media-list li a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: #fff;
    }

    .social-media-list li a img {
      width: 20px;
      height: 20px;
      margin-right: 5px;
    }

    .terms-list {
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top: 10px;
    }

    .terms-list li {
      margin-right: 10px;
    }

    .terms-list li:last-child {
      margin-right: 0;
    }

    .terms-list li a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: #fff;
    }

    .terms-list li a img {
      width: 20px;
      height: 20px;
      margin-right: 5px;
    }
  </style>
</head>
<body>
  <div class="banner">
    <div>
      <div class="banner-content">
        <h1 class="banner-title">
          <span class="highlight">Salve ! </span>
        </h1>
        <h5 class="banner-subtitle">Click on the below button to get into FERRARI FAMILY</h5>
        <button class="banner-button" onclick="toggleRegistrationForm()">Get started</button>
        <!-- Registration Form -->
        <div class="registration-form" id="registrationForm">
          <div class="registration-form-inner">
            <h2>Create Account</h2>
            <form>
              <label for="username">Create Username</label>
              <input type="text" id="username" name="username" required>

              <label for="password">Create Password</label>
              <input type="password" id="password" name="password" required>

              <button type="submit">Sign Up</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>

  <script>
    function toggleRegistrationForm() {
      const registrationForm = document.getElementById("registrationForm");
      registrationForm.classList.toggle("open");
    }
  </script>

  <header>
    <div class="menu-icon" onclick="document.querySelector('.menu').classList.toggle('open')">
      <div class="menu-line"></div>
      <div class="menu-line"></div>
      <div class="menu-line"></div>
      <span color="white">Menu</span>
    </div>
    <div class="menu">
      <ul>
        <li><a href="fabout.html">ABOUT</a></li>
        <li><a href="polo-shirt.html">FEATURED CARS</a></li>
        
      </ul>
    </div>
  </header>
  <section>
    <h2>Featured People</h2>
    <section>
        <div class="person-grid">
          <div class="person">
            <img src="raja.jpeg" alt="Person 1">
            <h3>Raja R</h3>
            <address>Saveetha Nagar, Chennai - India</address>
          </div>
          <div class="person">
            <img src="Enzo-Ferrari.jpg" alt="person2">
            <h3>Enzo Ferrari</h3>
            <address>Maranello, Italy</address>
          </div>
        </div>
      </section>
      
  </section>

  <footer>
    <div class="footer-content">
      <div class="footer-column">
        <h4>Social Media</h4>
        <ul class="social-media-list">
          <li>
            <a href="https://www.instagram.com/eswar_018_/?igshid=NTc4MTIwNjQ2YQ%3D%3D">
              <img src="insta logo-fotor-bg-remover-2023052412530.png" alt="Instagram Logo">
              Instagram
            </a>
          </li>
        </ul>
      </div>
      
      <div class="footer-column">
        <h4>Contact Information</h4>
        <p>Email: ferrariofficial@gmail.com</p>
        <p>Phone: 123-456-7890</p>
        <p>Address: Saveetha Nagar, Thandalam, Chennai</p>
      </div>
      <div class="footer-column">
        <div class="column">

        <h4>Legal</h4>
        <ul class="terms-list">
          <li>
            <a href="terms.html">
            <img src="accept.png" alt="Terms logo">
            Terms and Condition
          </a>
        </li>
        </ul>
      </div>
      
    </div>
    
  </footer>

</body>
</html>
```
### model.html
```
<!DOCTYPE html>
<html>
<head>
  <title>Models</title>
  <link rel="stylesheet" type="text/css" href="style.css">
  <style>
    img {
      max-width: 100%;
      height: auto;
      display: block;
      max-height: 700px; /* Adjust the value as needed */
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <ul class="menu">
        <li><a href="findex.html">Home</a></li>
        <li><a href="fabout.html">About</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <div class="menu">
      <ul>
        <li><a href="fabout.html">ABOUT</a></li>
        <li><a href="polo-shirt.html">FEATURED CARS</a></li>
        
      </ul>
    </div>
    <section id="polo-shirt">
      
      <h2>MODEL 1</h2>
      
        <div class="product-grid">
          <div class="product">
            <div class="img">
              <img src="ferrarimodel3.jpg" alt="Ferrari F40" height="100px">
            </div>
            <h3>Ferrari F40</h3>
            <p>Step into the family of Ferrari through Ferrari F40 where you redeem your respect without much effect.</p>
            <button>$2,266,757</button>
          </div>
          
            </div>
        <!-- Add more polo shirt elements here -->
      </div>
    </section>
    <section id="polo-shirt2">
      <h2>MODEL 2</h2>
      
        <div class="product-grid">
          <div class="product">
            <div class="img">
              <img src="Untitledferrari.jpg" alt="Ferrari F40" height="100px">
            </div>
            <h3>Ferrari F10 ROADSTER</h3>
            <p>Rock your public road with Ferrari F10 roadster.With bloodmoon red in colour ,ferrari F10 will pull dollis for 101% sure</p>
            <button>$1,100,850</button>
          </div>
          
            </div>
        <!-- Add more polo shirt elements here -->
      </div>
    </section>
  </main>

  <footer>
    &copy; 2023 Ferrari. All rights reserved.
  </footer>
</body>
</html>
```

## OUTPUT:
![Screenshot from 2023-06-03 23-25-23](https://github.com/Raja8334/productcompanywebsite/assets/120719634/cd25a304-33fe-4614-a405-2417721928e0)

### Home Page:
![IMG-20230606-WA0007](https://github.com/Raja8334/productcompanywebsite/assets/120719634/367f2085-75b4-4e56-988a-7846990f3c87)
![IMG-20230606-WA0003](https://github.com/Raja8334/productcompanywebsite/assets/120719634/e8e4ef27-5715-4ceb-8a2c-c7066e3f76ba)

### About:
![IMG-20230606-WA0009](https://github.com/Raja8334/productcompanywebsite/assets/120719634/9267bb1a-51d0-4af3-ae5f-904f9826039a)
### People:
![IMG-20230606-WA0006](https://github.com/Raja8334/productcompanywebsite/assets/120719634/8cc22529-54b3-4018-83d2-08aa50743a2d)
### Product:
![IMG-20230606-WA0008](https://github.com/Raja8334/productcompanywebsite/assets/120719634/0d6ab591-401d-44b9-93e5-f92cf5456412)

## Result:

Thus a website is designed for the software product company and the HTML,CSS code are validated.
