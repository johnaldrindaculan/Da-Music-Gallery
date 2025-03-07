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
