<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Blog | Explore Musical Instruments</title>
    <link rel="stylesheet" href="styles.css">
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

   <script src="script.js"></script>
</body>
</html>
