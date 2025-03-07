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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Blog</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        header {
            background: #35424a;
            color: #ffffff;
            padding-top: 30px;
            min-height: 70px;
            border-bottom: #e8491d 3px solid;
        }
        header a {
            color: #ffffff;
            text-decoration: none;
            text-transform: uppercase;
            font-size: 16px;
        }
        #main {
            padding: 20px;
            background: #ffffff;
        }
        #comments-section {
            margin-top: 20px;
        }
        .comment {
            background: #e4e4e4;
            margin-bottom: 10px;
            padding: 10px;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>My Music Blog</h1>
        </div>
    </header>
    <div id="main" class="container">
        <h2>Welcome to My Music Blog</h2>
        <p>Feel free to share your thoughts about the latest music releases!</p>
        
        <div id="comments-section">
            <h3>Comments</h3>
            <form id="comment-form">
                <input type="text" id="username" placeholder="Your Name" required>
                <textarea id="comment" placeholder="Your Comment" required></textarea>
                <button type="submit">Submit</button>
            </form>
            <div id="comments">
                <!-- Comments will be displayed here -->
            </div>
        </div>
    </div>

    <script>
        document.getElementById('comment-form').addEventListener('submit', function(e) {
            e.preventDefault();

            const username = document.getElementById('username').value;
            const comment = document.getElementById('comment').value;

            const commentSection = document.getElementById('comments');
            const commentDiv = document.createElement('div');
            commentDiv.className = 'comment';
            commentDiv.innerHTML = `<strong>${username}</strong><p>${comment}</p>`;

            commentSection.appendChild(commentDiv);

            document.getElementById('comment-form').reset();
        });
    </script>
</body>
</html>
# My Music Blog

- [Home](Home/README.md)
- [Genres](Genres/README.md)
- [About](About/README.md)
- [Contact](Contact/README.md)
