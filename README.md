<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Blog | Explore Musical Instruments</title>
    <style>
        body {
            background-color: black;
            color: gold;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

   header {
            text-align: center;
            padding: 20px;
            background-color: #222;
            color: gold;
        }

   nav {
            background-color: #333;
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
            color: gold;
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
            background: #111;
            padding: 15px;
            margin: 15px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(255, 215, 0, 0.5);
            text-align: left;
            max-width: 600px;
            margin: auto;
        }

   .blog-post img {
            width: 100%;
            max-width: 500px;
            border-radius: 5px;
            display: block;
            margin: auto;
        }

   .blog-post h3 {
            color: gold;
            text-align: center;
        }

   .blog-post a {
            display: inline-block;
            margin-top: 10px;
            padding: 8px 15px;
            background-color: gold;
            color: black;
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
            background-color: #222;
            color: gold;
            margin-top: 20px;
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
       <img src="https://johnaldrindaculan.github.io/music-blog/images/guitar.jpg" alt="Guitar">
            <h3>The Guitar</h3>
            <p><strong>Definition:</strong> A stringed instrument played by plucking or strumming.</p>
            <p><strong>History:</strong> The guitar has roots dating back over 4,000 years, with early versions appearing in ancient Persia and Egypt.</p>
            <p><strong>Use:</strong> Found in many genres, from classical to rock and pop.</p>
            <a href="posts/guitar.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="https://johnaldrindaculan.github.io/music-blog/images/piano.html" alt="Piano">
            <h3>The Piano</h3>
            <p><strong>Definition:</strong> A keyboard instrument where hammers strike strings to produce sound.</p>
            <p><strong>History:</strong> Invented in Italy in the early 1700s by Bartolomeo Cristofori.</p>
            <p><strong>Use:</strong> Essential in classical, jazz, and contemporary music.</p>
            <a href="posts/piano.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="https://johnaldrindaculan.github.io/music-blog/images/violin.html" alt="Violin">
            <h3>The Violin</h3>
            <p><strong>Definition:</strong> A bowed string instrument with four strings.</p>
            <p><strong>History:</strong> Originated in the 16th century in Italy, evolving from earlier stringed instruments.</p>
            <p><strong>Use:</strong> Key in orchestras, folk music, and solo performances.</p>
            <a href="posts/violin.html">Read More</a>
        </div>

   <div class="blog-post">
       <img src="https://johnaldrindaculan.github.io/music-blog/images/drums.jpg" alt="Drums">
            <h3>The Drums</h3>
            <p><strong>Definition:</strong> A percussion instrument that produces sound when struck.</p>
            <p><strong>History:</strong> Drums have been used since ancient times for communication and music.</p>
            <p><strong>Use:</strong> Provides rhythm in nearly all genres of music.</p>
            <a href="posts/drums.html">Read More</a>
        </div>

   <div class="blog-post">
<img src="https://johnaldrindaculan.github.io/music-blog/images/flute.jpg" alt="Flute">
            <h3>The Flute</h3>
            <p><strong>Definition:</strong> A wind instrument that produces sound by blowing air across an opening.</p>
            <p><strong>History:</strong> One of the oldest musical instruments, with versions found in prehistoric times.</p>
            <p><strong>Use:</strong> Used in orchestras, folk music, and even pop and jazz.</p>
            <a href="posts/flute.html">Read More</a>
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
        <p id="formMessage"></p>
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
                document.getElementById("formMessage").style.color = "green";
                document.getElementById("contactForm").reset();
            } else {
                document.getElementById("formMessage").textContent = "Please fill out all fields.";
                document.getElementById("formMessage").style.color = "red";
            }
        });
    </script>

</body>
</html>
