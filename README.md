# Introduction to CSS

## Objectives
Link an external CSS file to an HTML document.
Apply basic styling using selectors.
Use colors, fonts, and spacing effectively.

## Instructions

Create a style.css file.
Apply CSS to a HTML page.
Style elements using:
Classes and IDs.
Color and typography.
Margins, paddings, and borders.

>[!NOTE]
>  - Include at least:
>  - Use of 3 selectors
>  - Style an image
>  - Margin, Padding & Borders
>  - Different font

# Tasks
 - Link an external CSS file.
 - Apply at least 3 different selectors.
 - Improve readability and aesthetics.

Happy Coding! 💻✨






<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Styled Page</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <header class="page-header">
        <h1 id="main-title" class="main-title">Welcome to My Awesome Page</h1>
        <p class="tagline header-tagline">A place for interesting things.</p>
    </header>

    <main class="main-content">
        <div class="container content-container">
            <img src="placeholder.jpg" alt="A placeholder image" class="placeholder-image">
            <section id="introduction" class="introduction-section">
                <h2 class="section-title">About Us</h2>
                <p class="paragraph introduction-paragraph">This is a paragraph introducing our amazing website. We strive to provide valuable content and a great user experience.</p>
                <p class="highlight introduction-highlight">Stay tuned for more updates!</p>
            </section>
        </div>
    </main>

    <footer class="page-footer">
        <p class="footer-text">&copy; 2025 My Awesome Page</p>
    </footer>
</body>
</html>
```css
/* General Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box; /* Include padding and border in element's total width/height */
}

body {
    font-family: 'Open Sans', sans-serif; /* More modern, readable font */
    line-height: 1.7;  /* Improved line height for better readability */
    background-color: #f9f9f9; /* Slightly warmer background */
    color: #444; /* Slightly darker, more readable text */
}

img {
    max-width: 100%; /* Responsive images */
    height: auto;
    display: block; /*removes extra space below image*/
}

/* Reusable styles (Can be applied to multiple elements) */
.container {
    max-width: 960px; /* Slightly wider, more standard max-width */
    margin: 0 auto; /* Center horizontally */
    padding: 20px;
}

.section-title {
    font-size: 2.2em; /* Larger section titles */
    color: #2c3e50; /* Darker heading color */
    margin-bottom: 25px; /* Increased margin below heading */
    text-align: center; /* Center align headings */
}

.paragraph{
    margin-bottom: 20px;
}

/* Header Section Styles */
.page-header {
    background-color: #34495e; /* Darker header background */
    color: #ffffff;
    padding: 25px 0; /* Increased vertical padding */
    text-align: center;
    margin-bottom: 30px; /* Add margin below header */
}

.main-title {
    font-size: 3em; /* Larger main title */
    margin-bottom: 15px;
    font-weight: 700; /* Use the bold weight of Open Sans */
}

.header-tagline {
    font-style: italic;
    color: #ecf0f1; /* Lighter tagline color */
    font-size: 1.1em;
}

/* Main Content Styles */
.content-container {
    background-color: #ffffff;
    padding: 30px; /* Increased padding inside container */
    border-radius: 10px; /* More rounded corners */
    box-shadow: 0 4px 15px rgba(0,0,0,0.1); /* Slightly stronger shadow */
}

.placeholder-image {
    margin-bottom: 25px;
    border: 8px solid #bdc3c7; /* Lighter border */
    border-radius: 10px;
}

.introduction-section {
    margin-bottom: 30px;
}


.introduction-paragraph {
    line-height: 1.7;
    color: #555;
}

.introduction-highlight {
    font-weight: 600; /* Use a semi-bold weight */
    color: #2980b9; /* A brighter highlight color */
    padding: 12px 18px;
    background-color: #e6f7ff;
    border-radius: 6px;
    margin-top: 15px;
    display: inline-block;
}

/* Footer Styles */
.page-footer {
    text-align: center;
    padding: 25px 0;
    background-color: #34495e; /* Darker footer */
    color: #ffffff;
    font-size: 0.95em;
    margin-top: 30px;
}
.footer-text{
    opacity: 0.8;
}

