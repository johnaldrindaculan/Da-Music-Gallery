# My Music Blog

Welcome to my music blog! This blog is dedicated to exploring various music genres, sharing insights, and connecting with fellow music enthusiasts. Whether you're a fan of rock, jazz, classical, or pop, you'll find something here to pique your interest. Dive in, explore, and enjoy!

## Table of Contents
- [Home](#home)
- [Genres](#genres)
- [About](#about)
- [Contact](#contact)
- [Contributing](#contributing)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #f4f4f4;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            max-width: 800px;
        }
        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 5px;
        }
        .gallery-item {
            flex: 1 1 calc(33.333% - 10px);
            box-sizing: border-box;
        }
        @media (max-width: 768px) {
            .gallery-item {
                flex: 1 1 calc(50% - 10px);
            }
        }
        @media (max-width: 480px) {
            .gallery-item {
                flex: 1 1 100%;
            }
        }
    </style>
</head>
<body>
    <div class="gallery">
        <div class="gallery-item">
            <img src="path/to/your/image1.jpg" alt="Image 1">
        </div>
        <div class="gallery-item">
            <img src="path/to/your/image2.jpg" alt="Image 2">
        </div>
        <div class="gallery-item">
            <img src="path/to/your/image3.jpg" alt="Image 3">
        </div>
        <!-- Add more images as needed -->
    </div>
</body>
</html>
