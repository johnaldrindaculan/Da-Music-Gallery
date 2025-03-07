<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Blog | Explore Musical Instruments</title>
    <style>
        /* Apply black background and gold font */
        body {
            background-color: black;
            color: gold;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

   /* Header */
        header {
            text-align: center;
            padding: 20px;
            background-color: #222;
            color: gold;
        }

   /* Navigation */
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

   /* Sections */
        section {
            padding: 20px;
            text-align: center;
        }

   /* Blog Post Styling */
        .blog-post {
            background: #111;
            padding: 15px;
            margin: 15px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(255, 215, 0, 0.5);
        }

   .blog-post img {
            width: 100%;
            max-width: 500px;
            border-radius: 5px;
        }

   .blog-post h3 {
            color: gold;
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

   /* Contact Form */
        form {
            display: flex;
            flex-direction: column;
            max-width: 400px;
            margin: auto;
        }

   input, textarea {
            margin: 10px 0;
            padding: 10px;
            width: 100%;
            border: 1px solid gold;
            background: black;
            color: gold;
            border-radius: 5px;
        }

   button {
            background-color: gold;
            color: black;
            padding: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            font-weight: bold;
        }

   button:hover {
            background-color: white;
            color: black;
        }

   /* Footer */
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
            <img src="images/guitar.jpg" alt="Guitar">
            <h3>The Timeless Charm of the Guitar</h3>
            <p>Learn why the guitar remains one of the most popular musical instruments worldwide...</p>
            <a href="posts/guitar.html">Read More</a>
        </div>

   <div class="blog-post">
            <img src="images/piano.jpg" alt="Piano">
            <h3>The Magic of Piano Music</h3>
            <p>Discover how the piano has shaped classical and modern music...</p>
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
