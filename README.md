# My Music Blog

Welcome to my music blog! Here you can find various sections:

- [Home](Home/README.md)
- [Genres](Genres/README.md)
- [About](About/README.md)
- [Contact](Contact/README.md)

# Home
Welcome to the Home section of my music blog!
# Genres
Explore different music genres here!
# About
Learn more about the blog and the author.
# Contact
Get in touch with me through this section!

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
                <li><a href="#" onclick="showContent('home')">Home</a></li>
                <li><a href="#" onclick="showContent('genres')">Genres</a></li>
                <li><a href="#" onclick="showContent('about')">About</a></li>
                <li><a href="#" onclick="showContent('contact')">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main id="content">
        <!-- Content will be displayed here -->
    </main>
    <footer>
        <p>&copy; 2025 My Music Blog. All rights reserved.</p>
    </footer>
    <script src="js/scripts.js"></script>
</body>
</html>

function showContent(section) {
    const content = document.getElementById('content');
    let text = '';

    switch (section) {
        case 'home':
            text = '<h2>Welcome to My Music Blog</h2><p>This is the home section where you can find the latest updates and news.</p>';
            break;
        case 'genres':
            text = '<h2>Genres</h2><p>Explore different music genres here!</p>';
            break;
        case 'about':
            text = '<h2>About</h2><p>Learn more about the blog and the author.</p>';
            break;
        case 'contact':
            text = '<h2>Contact</h2><p>Get in touch with me through this section!</p>';
            break;
        default:
            text = '<h2>Welcome to My Music Blog</h2>';
    }

    content.innerHTML = text;
}
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
