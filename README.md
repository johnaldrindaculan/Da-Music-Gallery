# my-music-blog
my-music-blog/
├── index.html
├── css/
│   └── styles.css
├── js/
│   └── scripts.js
└── images/
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Music Blog</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>My Music Blog</h1>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Genres</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="blog-posts">
            <!-- Blog posts will go here -->
        </section>
        <section id="music-player">
            <!-- Music player will go here -->
        </section>
    </main>
    <footer>
        <p>&copy; 2025 My Music Blog. All rights reserved.</p>
    </footer>
    <script src="js/scripts.js"></script>
</body>
</html>
/* css/styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}
header {
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
    text-align: center;
}
nav ul {
    list-style: none;
    padding: 0;
}
nav ul li {
    display: inline;
    margin: 0 10px;
}
nav ul li a {
    color: #fff;
    text-decoration: none;
}
main {
    padding: 20px;
}
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    bottom: 0;
    width: 100%;
}
