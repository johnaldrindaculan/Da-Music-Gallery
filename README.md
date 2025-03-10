<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Blog | Explore Musical Instruments</title>
    <style>
        body {
            background: url('images/images (6).jpeg'); 
            background-size: cover; 
            background-position: center; 
            background-attachment: fixed; 
            background-repeat: no-repeat; 
            color: #FFD700; 
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

   header {
            text-align: center;
            padding: 20px;
            background-color: black;
            color: #FFD700; 
        }

   nav {
            background-color: black;
            padding: 10px;
            text-align: center;
        }

   nav ul {
            list-style: none;
            padding: 0;
        }

   nav ul li {
            display: inline;
            margin: 0 15px;
        }

   nav ul li a {
            color: #FFD700; 
            text-decoration: none;
            font-weight: bold;
        }

   nav ul li a:hover {
            color: white;
        }

   section {
            padding: 20px;
            text-align: center;
        }

   .blog-post {
            background: #FFD700; 
            padding: 15px;
            margin: 15px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(255, 215, 0, 0.5);
            text-align: left;
            max-width: 600px;
            margin: auto;
            color: black; 
        }

   .blog-post img {
            width: 100%;
            max-width: 500px;
            border-radius: 5px;
            display: block;
            margin: auto;
        }

   .blog-post h3 {
            color: black;
            text-align: center;
        }

   .blog-post a {
            display: inline-block;
            margin-top: 10px;
            padding: 8px 15px;
            background-color: black;
            color: #FFD700;
            text-decoration: none;
            border-radius: 5px;
        }

   .blog-post a:hover {
            background-color: white;
            color: black;
        }

   footer {
            text-align: center;
            padding: 15px;
            background-color: black;
            color: #FFD700; 
            margin-top: 20px;
        }

   form {
            background: black; 
            padding: 20px;
            border-radius: 5px;
            color: #FFD700; 
            max-width: 400px;
            margin: auto;
            border: 2px solid #FFD700; 
        }

   label {
            display: block;
            margin: 10px 0 5px;
        }

   input, textarea {
            width: 100%;
            padding: 8px;
            margin: 5px 0 15px;
            border-radius: 5px;
            border: 1px solid #FFD700;
            background: black;
            color: #FFD700;
        }

   button {
            background-color: black;
            color: #FFD700;
            border: 2px solid #FFD700;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
        }

   button:hover {
            background-color: #FFD700;
            color: black;
        }
    </style>
</head>
<body>

  <header>
        <h1>Music Blog</h1>
        <p>Discover the beauty of musical instruments</p>
    </header>

   <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#blog">Blog</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

   <section id="blog">
        <h2>Latest Blog Posts</h2>

   <div class="blog-post">
            <img src="images/images (8).jpeg" alt="Guitar">
            <h3>The Guitar</h3>
            <a href="posts/guitar.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/images (9).jpeg" alt="Piano">
            <h3>The Piano</h3>
            <a href="posts/piano.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/download.jpeg" alt="Violin">
            <h3>The Violin</h3>
            <a href="posts/violin.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/images (10).jpeg" alt="Drums">
            <h3>The Drums</h3>
            <a href="posts/drums.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/images (11).jpeg" alt="Flute">
            <h3>The Flute</h3>
            <a href="posts/flute.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/images (13).jpeg" alt="Saxophone">
            <h3>The Saxophone</h3>
            <a href="posts/saxophone.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/download (6).jpeg" alt="Trumpet">
            <h3>The Trumpet</h3>
            <a href="posts/trumpet.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/download (7).jpeg" alt="Cello">
            <h3>The Cello</h3>
            <a href="posts/cello.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/download (8).jpeg" alt="Harp">
            <h3>The Harp</h3>
            <a href="posts/harp.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/download (9).jpeg" alt="Accordion">
            <h3>The Accordion</h3>
            <a href="posts/accordion.html">Read More</a>
        </div>
    </section>

   <section id="contact">
        <h2>Contact Us</h2>
        <form id="contactForm">
            <label for="name">Name:</label>
            <input type="text" id="name" required>

   <label for="email">Email:</label>
            <input type="email" id="email" required>

   <label for="message">Message:</label>
            <textarea id="message" required></textarea>

   <button type="submit">Send</button>
        </form>
        <p id="formMessage" style="text-align: center; margin-top: 10px;"></p>
    </section>

   <footer>
        <p>&copy; 2025 Music Blog. All rights reserved.</p>
    </footer>

   <script>
        document.getElementById("contactForm").addEventListener("submit", function(event) {
            event.preventDefault();
            let name = document.getElementById("name").value;
            let email = document.getElementById("email").value;
            let message = document.getElementById("message").value;

            if (name && email && message) {
                document.getElementById("formMessage").textContent = "Thank you for your message!";
                document.getElementById("contactForm").reset();
            } else {
                document.getElementById("formMessage").textContent = "Please fill out all fields.";
                document.getElementById("formMessage").style.color = "red";
            }
        });
    </script>
</body>
</html>
