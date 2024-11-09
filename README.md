# https://gabrielecossutta.github.io/

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Page responsive on mobile -->
    <title>Portfolio - My Projects</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet"> <!-- Link to the font -->
    <style> /* CSS */
```css
        * {
            box-sizing: border-box; /* Sets box-sizing to include padding and border in width/height */
            margin: 0; /* Remove margin */
            padding: 0; /* Remove padding */
        }
        body {
            font-family: 'Roboto', sans-serif;  /* Set the fonts for all the body */
            background-color: #f4f7fa; /* Background color*/
            color: #333; /* Text color */
            display: flex; /* Facilitate page alignment */ 
            flex-direction: column;
            align-items: center;
        }
        header { /* Headear */
            background: linear-gradient(135deg, #6f86d6, #48c6ef); /* Background color */
            color: #fff; /* Text color */
            padding: 60px 0; /* Padding at the top and bottom */
            text-align: center; /* Center Text*/
            width: 100%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2); /* Shadow */
        }
        header h1 { /* Headear 1 */
            font-size: 3.2em; /* Font size */
            margin-bottom: 10px; /* Spacing */
            font-weight: 700; /* Bold */
        }
        header p { /* Paragraph */
            font-size: 1.3em; /* Font size */
            margin-top: 5px; /* Spacing */
        }
        /* Classes */
        .container {
            max-width: 1200px; /* Maximum width */
            width: 90%; /* Width */
            margin: 40px auto; /* Spacing */
            display: flex;
            flex-direction: column;
            gap: 30px; /* Space between projects */
        }
        .project {
            display: flex;
            align-items: center; /* Vertically centers image and content */
            justify-content: space-between; /* Distributes image and text to the sides */
            background-color: #fff; /* Background */
            border-radius: 12px; /* Rounds the edges */
            overflow: hidden; /* Hides any content outside the borders */
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1); /* Shadow */
            transition: transform 0.3s, box-shadow 0.3s; /* Animation */
            padding: 20px; /* Inner spacing */
            text-align: center;
        }
        .project:hover {
            transform: translateY(-10px); /* Animation */
            box-shadow: 0 16px 30px rgba(0, 0, 0, 0.2); /* Shadow */
        }
        .project img {
            width: 250px; /* Width */
            height: 170px; /* Height */
            object-fit: cover; /* Fits the image in the container */
            margin-right: 20px; /* Spacing */
        }
        .project-content {
            display: flex;
            flex-direction: column;
            justify-content: center;
            flex: 1;
        }
        .project h2 { /* Headear 2 */
            font-size: 1.5em; /* Font size */
            color: #333f58; /* Text color */
            margin-bottom: 10px; /* Spacing */
        }
        .project p { /* Paragraph */
            color: #666; /* Text color */
            font-size: 1em; /* Font size */
            margin: 15px 0; /* Spacing */
            line-height: 1.6;
        }
        .details {
            text-align: center; /* Centers the text*/
            margin-left: 20px; /* Spacing*/
        }
        .details h3 { /* Headear 3 */
            margin-bottom: 5px; /* Spacing */
            font-size: 1em; /* Font size */
            color: #333f58; /* Text color */
        }
        .details p { /* Paragraph */
            font-size: 1.2em; /* Font size */
            color: #333f58; /* Text color */
        }
        .project a { /* Anchor */
            padding: 10px 20px; /* Spacing */
            color: #fff; /* Text color*/
            background-color: #ef8354; /* Background color  */
            border-radius: 30px; /* Rounds the edges */
            font-weight: 600; /* Bold */
            text-decoration: none; /* Removes underline */
            transition: background-color 0.3s, transform 0.3s; /* Animation */
            margin-top: 10px; /* Spacing */
            align-self: center;
        }
        .project a:hover {
            background-color: #d94d28; /* Button color on hover */
            transform: scale(1.05); /* Slightly scales up on hover */
        }
        footer {
            margin-top: 40px; /* Spacing */
            padding: 20px; /* Spacing */
            text-align: center; /* Centers the text */
            width: 100%;
            background-color: #333f58; /* Background color */
            color: #fff; /* Text color */
            font-size: 0.9em; /* Font size */
            cursor: pointer; /* Changes cursor to indicate it is clickable */
        }
        footer p {
            color: #b0c4de; /* Text color */
        }
```html
    </style>
</head>
<body id="top">
    <header>
        <h1>My Projects</h1> <!-- Main title of the page -->
        <p>Explore my portfolio! Check out my latest projects.</p>
    </header>
    <div class="container"> <!-- Main container for projects -->
        <div class="project"> <!-- Start of a project -->
            <img src="img/test.jpg"> <!-- Project image -->
            <div class="project-content"> <!-- Container for project content -->
                <<h2>This Web Site</h2>
        	<p>The html and css code of this site.</p>
                <a href="https://github.com/gabrielecossutta/gabrielecossutta.github.io?tab=readme-ov-file" target="_blank">Look on GitHub</a>
            </div>
            <div class="details"> <!-- Container for details level -->
		<h3>Skills</h3> <!-- Title for details level -->
                <p>HTML - CSS</p>
                <h3>Level of Completion</h3> <!-- Title for details level -->
                <p>10/10</p>
            </div>
        </div>
    </div>
    <footer onclick="scrollToTop()">
        <p>Back to Top</p>
    </footer>

    <script>
        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }
    </script>
</body>
</html>