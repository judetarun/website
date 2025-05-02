# Ex.07 Restaurant Website
# Date:1.05.25
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
project.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>FORK & FLAME| Home-Cooked Delights</title>
    <link rel="icon" href="background.png">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            background-image: url('background.png');
            background-repeat: no-repeat;
            background-size: cover;
            color: rgb(243, 36, 17);
            margin: 0;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
            text-align: center;
        }

        .nav-list {
            background-color: rgba(0, 0, 0, 0.6);
            padding: 15px;
        }

        .nav-list a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
        }

        .nav-list a:hover {
            text-decoration: underline;
        }

        h1 {
            color: rgb(255, 174, 22);
            font-size: 50px;
            margin-top: 20px;
        }

        img {
            height: 200px;
            margin-top: 20px;
        }

        .discount-banner {
            background-color: #e71515;
            color: rgb(6, 6, 5);
            padding: 15px 30px;
            text-align: center;
            font-size: 20px;
            font-weight: bold;
            border-radius: 8px;
            margin: 20px auto;
            width: fit-content;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            font-family: cursive;
        }

        .our-story {
            background-color: rgba(243, 117, 13, 0.85);
            color: #000000;
            padding: 30px;
            margin: 30px auto;
            width: 80%;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
            text-align: center;
            font-family: cursive;
        }

        .our-story h2 {
            font-size: 32px;
            margin-bottom: 15px;
            color: #000000;
            font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
        }

        .our-story p {
            font-size: 18px;
            line-height: 1.6;
        }

        .featured-dishes {
            background-color: rgba(235, 102, 7, 0.958);
            color: #2b2b2b;
            padding: 40px 20px;
            margin: 20px auto;
            width: 90%;
            border-radius: 12px;
        }

        .featured-dishes h2 {
            font-size: 32px;
            margin-bottom: 30px;
            color: #000000;
        }

        .dish-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .dish-card {
            background-color: #ca6624;
            color: #000;
            padding: 20px;
            width: 250px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.15);
            text-align: center;
        }

        .dish-card img {
            width: 100%;
            height: 150px;
            border-radius: 8px;
            object-fit: cover;
            margin-bottom: 10px;
        }

        .dish-card h3 {
            margin: 10px 0 5px;
            color: #e09b10;
        }

        .dish-card p {
            font-size: 15px;
        }

        @media (max-width: 600px) {
            .dish-grid {
                flex-direction: column;
                align-items: center;
            }

            img {
                height: 120px;
            }
        }
    </style>
</head>
<body>
    <nav class="nav-list">
        <a href="#">Home</a>
        <a href="menu.html">Menu</a>
        <a href="contact.html">Contact</a>
        <a href="Administration.html">Administration</a>
    </nav>

    <img src="flame logo.png" alt="Fork & Flame Logo">
    <h1>Ｆｏｒｋ ＆ Ｆｌａｍｅ</h1>
    

    <div class="discount-banner">
        Photo Challenge: Post a dish and tag the restaurant to win a free Dessert.
    </div>

    <div class="our-story">
        <h2>Our Story</h2>
        <p>
            Fork & Flame Hotel is a modern, stylish boutique property designed for travelers seeking comfort, character, and culinary excellence.
             It blends industrial-chic design with warm, fiery accents, offering guests an immersive sensory experience from check-in to checkout.
        </p>
    </div>

    <div class="featured-dishes">
        <h2>Featured Dishes</h2>
        <div class="dish-grid">
            <div class="dish-card">
                <img src="smoked chicken wings.jpg" alt="Smoked Chicken Wings">
                <h3>Smoked Chicken Wings</h3>
                <p>Dry-rubbed and slow-smoked, finished over open flame, served with charred lime and chipotle ranch.</p>
            </div>
            <div class="dish-card">
                <img src="Pulled Chicken Sliders.jpeg" alt="Pulled Chicken Sliders">
                <h3>Pulled Chicken Sliders</h3>
                <p>Hickory-smoked chicken on mini brioche buns with flame-roasted jalapeño slaw.</p>
            </div>
            <div class="dish-card">
                <img src="grill.jpg" alt="Fire-Grilled Chicken Skewers ">
                <h3>Fire-Grilled Chicken Skewers </h3>
                <p>Marinated in garlic, yogurt, and lemon; served with burnt chili dip.</p>
            </div>
            <div class="dish-card">
                <img src="Korean Fire Chicken.png" alt="Korean Fire Chicken">
                <h3>Korean Fire Chicken</h3>
                <p>Gochujang-marinated grilled chicken with blistered scallions, kimchi slaw, and sesame.</p>
            </div>
        </div>
    </div>
</body>
</html>
```
menu.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Fork & Flame Menu</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #fffaf3;
      color: #2d2d2d;
      margin: 0;
      padding: 20px;
    }

    h1 {
      text-align: center;
      color: #e25822;
    }

    details {
      background-color: #fff;
      border: 1px solid #e25822;
      border-radius: 8px;
      margin: 10px 0;
      padding: 10px 15px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    summary {
      font-size: 20px;
      font-weight: bold;
      cursor: pointer;
      color: #e25822;
    }

    .item {
      padding: 10px 0;
      border-bottom: 1px solid #eee;
    }

    .item:last-child {
      border-bottom: none;
    }

    .item-name {
      font-weight: 600;
    }

    .item-description {
      font-size: 14px;
      color: #555;
    }

    .item-price {
      float: right;
      color: #000;
    }
  </style>
</head>
<body>

<h1>🔥 Fork & Flame Menu</h1>

<details open>
  <summary>Starters</summary>
  <div class="item">
    <span class="item-name">Smoked Chicken Wings</span>
    <span class="item-price">$8.99</span>
    <div class="item-description">Slow-smoked wings, flame-finished with chipotle ranch.</div>
  </div>
  <div class="item">
    <span class="item-name">Pulled Chicken Sliders</span>
    <span class="item-price">$7.99</span>
    <div class="item-description">Mini brioche sliders with hickory-smoked chicken and jalapeño slaw.</div>
  </div>
  <div class="item">
    <span class="item-name">BBQ Chicken Quesadilla</span>
    <span class="item-price">$9.49</span>
    <div class="item-description">Grilled tortilla stuffed with BBQ chicken, cheddar cheese, and caramelized onions. Served with smoky salsa.</div>
</div>
<div class="item">
    <span class="item-name">Crispy Chicken Lollipops</span>
    <span class="item-price">$8.99</span>
    <div class="item-description">Frenched chicken wings marinated and deep-fried, served with fiery dipping sauce.</div>
</div>
<div class="item">
    <span class="item-name">Tandoori Chicken Bites</span>
    <span class="item-price">$8.79</span>
    <div class="item-description">Boneless chunks marinated in traditional tandoori spices, grilled and served with mint chutney.</div>
</details>

<details>
  <summary>Mains</summary>
  <div class="item">
    <span class="item-name">Fire-Grilled Chicken Skewers</span>
    <span class="item-price">$13.99</span>
    <div class="item-description">Garlic lemon marinade, served with chili dip.</div>
  </div>
  <div class="item">
    <span class="item-name">Korean Fire Chicken</span>
    <span class="item-price">$14.99</span>
    <div class="item-description">Gochujang grilled chicken, kimchi slaw, and scallions.</div>
  </div>
  <div class="item">
    <span class="item-name">Flame-Roasted Chicken Platter</span>
    <span class="item-price">$15.99</span>
    <div class="item-description">Half chicken marinated in house spices, roasted over open flames, served with grilled veggies and garlic mash.</div>
</div>

<div class="item">
    <span class="item-name">Peri-Peri Chicken Bowl</span>
    <span class="item-price">$13.99</span>
    <div class="item-description">Spicy grilled chicken served over lemon rice with roasted corn, slaw, and peri-peri drizzle.</div>
</div>

<div class="item">
    <span class="item-name">Smoky BBQ Chicken Ribs</span>
    <span class="item-price">$17.49</span>
    <div class="item-description">Tender boneless chicken ribs slow-cooked in smoky BBQ sauce, served with flame fries.</div>
</div>

<div class="item">
    <span class="item-name">Creamy Chipotle Chicken Pasta</span>
    <span class="item-price">$14.99</span>
    <div class="item-description">Grilled chicken tossed in creamy chipotle sauce with penne, parmesan, and fire-roasted peppers.</div>
</div>

</details>

<details>
  <summary>Sides</summary>
  <div class="item">
    <span class="item-name">Flame Fries</span>
    <span class="item-price">$4.99</span>
    <div class="item-description">Tossed in chili salt, served with sriracha mayo.</div>
  </div>
  <div class="item">
    <span class="item-name">Smoky Garlic Bread</span>
    <span class="item-price">$3.99</span>
    <div class="item-description">Toasted with smoked garlic butter and herbs.</div>
  </div>
  <div class="item">
    <span class="item-name">Charred Corn on the Cob</span>
    <span class="item-price">$4.49</span>
    <div class="item-description">Flame-grilled corn brushed with chili-lime butter and sprinkled with smoked paprika.</div>
</div>

<div class="item">
    <span class="item-name">Spicy Flame Fries</span>
    <span class="item-price">$4.99</span>
    <div class="item-description">Crispy fries tossed in house chili salt, served with chipotle mayo.</div>
</div>

<div class="item">
    <span class="item-name">Grilled Veggie Medley</span>
    <span class="item-price">$5.99</span>
    <div class="item-description">A mix of zucchini, peppers, and onions fire-grilled and seasoned with herbs and garlic.</div>
</div>

<div class="item">
    <span class="item-name">Buttered Garlic Rice</span>
    <span class="item-price">$3.99</span>
    <div class="item-description">Steamed rice infused with roasted garlic and finished with a butter glaze.</div>
</div>
</details>

<details>
  <summary>Desserts</summary>
  <div class="item">
    <span class="item-name">Molten Lava Cake</span>
    <span class="item-price">$6.99</span>
    <div class="item-description">Hot chocolate cake with gooey center and vanilla ice cream.</div>
  </div>
  <div class="item">
    <span class="item-name">Grilled Pineapple Sundae</span>
    <span class="item-price">$5.99</span>
    <div class="item-description">Caramelized pineapple, ice cream, and toasted coconut.</div>
  </div>
</div>
<div class="item">
    <span class="item-name">Cinnamon Fire Churros</span>
    <span class="item-price">$4.99</span>
    <div class="item-description">Crispy churros dusted with chili cinnamon sugar, served with chocolate lava dip.</div>
</div>

<div class="item">
    <span class="item-name">S’mores Skillet Brownie</span>
    <span class="item-price">$6.49</span>
    <div class="item-description">A rich brownie topped with toasted marshmallows, graham crackers, and melted chocolate, served hot in a mini skillet.</div>
</div>

<div class="item">
    <span class="item-name">Honey Flame Bananas</span>
    <span class="item-price">$5.49</span>
    <div class="item-description">Flambéed bananas with honey-rum glaze, served with cinnamon ice cream.</div>
</div>
</details>

</body>
</html>
```
contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Contact Us | Fork & Flame</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: url('background.png') no-repeat center center fixed;
      background-size: cover;
      color: #fff;
      text-align: center;
    }

    .contact-container {
      background-color: rgba(0, 0, 0, 0.7);
      margin: 50px auto;
      padding: 40px;
      border-radius: 10px;
      width: 90%;
      max-width: 600px;
      box-shadow: 0 0 15px rgba(255, 69, 0, 0.5);
    }

    h1 {
      color: #ffa500;
      margin-bottom: 20px;
    }

    form input,
    form textarea {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: none;
      border-radius: 6px;
      font-size: 16px;
    }

    form button {
      background-color: #e25822;
      color: white;
      border: none;
      padding: 12px 20px;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
    }

    form button:hover {
      background-color: #ff4500;
    }

    .contact-info {
      margin-top: 30px;
      font-size: 16px;
    }

    .contact-info a {
      color: #ffd700;
      text-decoration: none;
    }

    .contact-info a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <div class="contact-container">
    <h1>Contact Fork & Flame</h1>
    <form action="mailto:your-email@example.com" method="post" enctype="text/plain">
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="email" name="email" placeholder="Your Email" required />
      <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>

    <div class="contact-info">
      <p><strong>Phone:</strong> +1 (555) 123-4567</p>
      <p><strong>Email:</strong> <a href="mailto:info@forkandflame.com">info@forkandflame.com</a></p>
      <p><strong>Address:</strong> 123 Fire Street, Flame City, FC 12345</p>
    </div>
  </div>
</body>
</html>
```
administration.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Our Chefs | Fork & Flame</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: url('background.png') no-repeat center center fixed;
      background-size: cover;
      color: #fff;
      text-align: center;
    }

    .container {
      background-color: rgba(0, 0, 0, 0.8);
      padding: 50px 20px;
      margin: 30px auto;
      max-width: 1000px;
      border-radius: 12px;
    }

    h1 {
      color: #ffa500;
      margin-bottom: 30px;
    }

    .chef-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
    }

    .chef-card {
      background-color: rgba(255, 255, 255, 0.05);
      border-radius: 10px;
      padding: 20px;
      width: 250px;
      box-shadow: 0 0 15px rgba(255, 69, 0, 0.5);
    }

    .chef-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
      margin-bottom: 15px;
      border: 3px solid #ff6600;
    }

    .chef-card h3 {
      color: #ffd700;
      margin: 10px 0 5px;
    }

    .chef-card p {
      font-size: 15px;
      color: #f1f1f1;
    }

    @media (max-width: 600px) {
      .chef-grid {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Meet Our Culinary Team</h1>

    <div class="chef-grid">
      <div class="chef-card">
        <img src="chef 1.avif" alt="Chef Marco">
        <h3>Chef Marco Blaze</h3>
        <p>Executive Chef & Grill Master with a love for fire-roasted perfection.</p>
      </div>

      <div class="chef-card">
        <img src="chef 2.jpg" alt="Chef stella jennifer">
        <h3>Chef stella jennifer</h3>
        <p>Pastry Chef bringing fiery flair to our desserts with molten lava treats.</p>
      </div>

      <div class="chef-card">
        <img src="chef 3.jpeg" alt="Chef Lee">
        <h3>Chef Daniel Lee</h3>
        <p>Fusion expert blending Asian spices with flame-grilled classics.</p>
      </div>

      <div class="chef-card">
        <img src="chef 4.png" alt="Chef leo">
        <h3>Chef leo Grant</h3>
        <p>Sous Chef ensuring every plate reflects Fork & Flame’s bold spirit.</p>
      </div>
    </div>
  </div>
</body>
</html>
```
# OUTPUT:
![Screenshot 2025-05-02 121526](https://github.com/user-attachments/assets/35a901a8-b512-4842-a81e-038d11756713)
![Screenshot 2025-05-02 121543](https://github.com/user-attachments/assets/bbc47c42-e0cd-4fdb-97b0-4170ff952f35)
![Screenshot 2025-05-02 121604](https://github.com/user-attachments/assets/43c1ddcc-0e5e-49db-9ecc-6b898705bad9)
![Screenshot 2025-05-02 121624](https://github.com/user-attachments/assets/ca5bf3d1-a0a4-4cfc-965c-a01622ed95b4)
![Screenshot 2025-05-02 121634](https://github.com/user-attachments/assets/2fa04cf5-669a-4529-973b-8fede9c5e8d1)
![Screenshot 2025-05-02 121649](https://github.com/user-attachments/assets/d03944d1-99bd-4a32-85af-e8cbec6b63e1)








# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
