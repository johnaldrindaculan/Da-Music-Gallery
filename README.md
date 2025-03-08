<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Blog | Explore Musical Instruments</title>
    <style>
        
   body {
            background: url('images/images (6).jpg'); 
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
            color: #FFD700; /* Gold */
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
            color: #FFD700; /* Gold */
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
            background: #FFD700; /* Yellow Gold */
            padding: 15px;
            margin: 15px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(255, 215, 0, 0.5);
            text-align: left;
            max-width: 600px;
            margin: auto;
            color: black; /* Black text for readability */
        }

   .blog-post img {
            width: 100%;
            max-width: 500px;
            border-radius: 5px;
            display: block;
            margin: auto;
        }

   .blog-post h3 {
            color: black; /* Black for readability */
            text-align: center;
        }

   .blog-post a {
            display: inline-block;
            margin-top: 10px;
            padding: 8px 15px;
            background-color: black;
            color: #FFD700; /* Gold */
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
            color: #FFD700; /* Gold */
            margin-top: 20px;
        }

        
   form {
            background: black; /* Black background */
            padding: 20px;
            border-radius: 5px;
            color: #FFD700; /* Gold text */
            max-width: 400px;
            margin: auto;
            border: 2px solid #FFD700; /* Gold border */
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
            border: 1px solid #FFD700; /* Gold border */
            background: black; /* Black input background */
            color: #FFD700; /* Gold text */
        }

   button {
            background-color: black;
            color: #FFD700; /* Gold */
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
            <p><strong>Definition:</strong> A stringed instrument played by plucking or strumming.</p>
            <p><strong>History:</strong> The guitar has roots dating back over 4,000 years, with early versions appearing in ancient Persia and Egypt.</p>
            <p><strong>Use:</strong> Found in many genres, from classical to rock and pop.</p>
            <a href="posts/guitar.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/images (9).jpeg" alt="Piano">
            <h3>The Piano</h3>
            <p><strong>Definition:</strong> A keyboard instrument where hammers strike strings to produce sound.</p>
            <p><strong>History:</strong> Invented in Italy in the early 1700s by Bartolomeo Cristofori.</p>
            <p><strong>Use:</strong> Essential in classical, jazz, and contemporary music.</p>
            <a href="posts/piano.html">Read More</a>
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
                document.getElementById("formMessage").style.color = "#FFD700"; // Gold text
                document.getElementById("contactForm").reset();
            } else {
                document.getElementById("formMessage").textContent = "Please fill out all fields.";
                document.getElementById("formMessage").style.color = "red";
            }
        });
    </script>

</body>
</html>
