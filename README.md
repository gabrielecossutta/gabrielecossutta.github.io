
### :arrow_down: To the website :arrow_down:
# https://gabrielecossutta.github.io/
### :arrow_up: To the website ⬆️

# HTML & CSS of the web site
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Portfolio - My Projects</title>
        <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet"> <!-- Link to the font -->
        <style>
            
            * { /* CSS */
                box-sizing: border-box; /* Sets box-sizing to include padding and border in width/height */
                margin: 0; /* Remove margin */
                padding: 0; /* Remove padding */
            }
    
            body {
                font-family: 'Roboto', sans-serif; /* Set the fonts for all the body */
                background-color: #1e1e1e; /* Background color*/
                color: #d3d3d3; /* Text color */
                display: flex; /* Facilitate page alignment */ 
                flex-direction: column; /* alignment direction*/ 
                align-items: center; /* center alignment */ 
                transition: background-color 0.3s, color 0.3s; /* Transition time */ 
            }
    
            header {
                background: linear-gradient(90deg, #ef8354, #000000); /* Background color left to right*/
                color: #f0f0f0; /* Text color */
                padding: 60px 0; /* Padding at the top and bottom */
                text-align: center; /* Center Text*/
                width: 100%; /* Occupies 100% of the container */
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
    
            .container {
                max-width: 1200px; /* Maximum width */
                width: 90%; /* Width */
                margin: 40px auto; /* Spacing */
                display: flex; /* Facilitate page alignment */
                flex-direction: column; /* alignment direction*/ 
                gap: 30px; /* Space between projects */
            }



            .cv-button { /* Change Theme icon */
                position: absolute; /*Absolute position, no container*/
                top: 20px; /* 20 pc from the top */
                left: 20px; /* 20 px from the left */
                width: 30px; /* Icon width */
                height: 30px; /* Icon height */
                cursor: pointer; /* Type of cursor*/
                transition: transform 0.3s; /* Animation Timer */
            }

            .cv-button:hover {
                transform: scale(1.5);/* Slightly scales up on hover */
            }
            
            .project {
                display: flex; /* Facilitate page alignment */
                align-items: center; /* Vertically centers image and content */
                justify-content: space-between; /* Distributes image and text to the sides */
                background-color: #333333; /* Background */
                color: #e1e1e1; /* Text color */
                border-radius: 12px; /* Rounds the edges */
                overflow: hidden; /* Hides any content outside the borders */
                box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1); /* Shadow */
                transition: transform 0.3s, box-shadow 0.3s; /* Animation */
                padding: 20px; /* Inner spacing */
                text-align: center; /* Text alignment */
            }
    
            .project:hover {
                transform: translateY(-10px); /* Animation */
                box-shadow: 0 16px 30px rgba(0, 0, 0, 0.2); /* Shadow */
                transform: scale(1.25); /* Slightly scales up on hover */
            }
    
            .project img {
                width: 250px; /* Width */
                height: 170px; /* Height */
                object-fit: cover; /* Fits the image in the container */
                margin-right: 20px; /* Spacing */
            }
    
            .project-content {
                display: flex;  /* Facilitate page alignment */
                flex-direction: column; /* alignment direction*/ 
                justify-content: center; /* Center elements */
                flex: 1; /* allows re-dimensioning of elements */
            }
    
            .project h2 { /* Headear 2 */
                font-size: 1.5em; /* Font size */
                color: #ef8354; /* Text color */
                margin-bottom: 10px; /* Spacing */
            }
    
            .project h3 {
                color: #ef8354; /* Text Color */
            }
    
            .project p { /* Paragraph */
                color: #b0c4de; /* Text color */
                font-size: 1em; /* Font size */
                margin: 15px 0; /* Spacing */
            }
    
            .project a { /* Anchor */
                padding: 10px 20px; /* Spacing */
                color: #ffffff; /* Text color*/
                background-color: #ef8354; /* Background color  */
                border-radius: 30px; /* Rounds the edges */
                font-weight: 600; /* Bold */
                text-decoration: none; /* Removes underline */
                transition: background-color 0.3s, transform 0.3s; /* Animation */
                margin-top: 10px; /* Spacing */
                align-self: center; /* alignment center */
            }

            .project a:hover {
                background-color: #d94d28; /* Button color on hover */
                transform: scale(1.05); /* Slightly scales up on hover */
            }
    
            .details { /* Colori delle descrizioni e dei dettagli */
                text-align: center; /* Centers the text*/
                width: 250px; /* Width */
                height: 170px; /* Height */
                color: #ef8354; /* Text color */
            }
    
            .details h3 {
                margin-bottom: 5px; /* Spacing */
                font-size: 1em; /* Font size */
                color: #ef8354; /* Text color */
            }
    
            .details p {
                font-size: 1.2em; /* Font size */
                color: #b0c4de; /* Text color */
            }
    
            .github-button {
                padding: 10px 20px; /* Spacing */
                background-color: #ef8354; /* Background color */
                color: #ffffff; /* Text color */
                border-radius: 30px; /* Rounds the edges */
                font-weight: 600; /* Bold */
                text-decoration: none; /* Removes underline */
                display: inline-block; /* Allows to treat it as inline block */
                transition: background-color 0.3s, transform 0.3s; /* Animation */
            }

            .github-button:hover {
                background-color: #d94d28; /* BackgroundColor */
                transform: scale(1.05); /* Slightly scales up on hover */
            }

            .back-to-top-button {
                padding: 10px 20px; /* Spacing */
                background-color: #ef8354; /* Background color */
                color: #ffffff; /* Text color */
                border-radius: 30px; /* Rounds the edges */
                font-weight: 600; /* Bold */
                text-decoration: none; /* Removes underline */
                display: inline-block; /* Allows to treat it as inline block */
                cursor: pointer; /* Change Cursor */
                transition: background-color 0.3s, transform 0.3s; /* Animation */
                text-align: center; /* Center Text */
                margin-top: 10px; /* Spacing */
            }
            
            .back-to-top-button:hover {
                background-color: #d94d28; /* BackgroundColor */
                transform: scale(1.05); /* Slightly scales up on hover */
            }

            .light-mode { /* Light mode */
                background-color: #f4f7fa; /* Background color */
                color: #333333; /* Text color */
            }

            .light-mode .project a:hover {
                background-color: #242d3f  ; /* Button color on hover */
                transform: scale(1.05); /* Slightly scales up on hover */
            }

            .light-mode header {
                background: linear-gradient(90deg, #333f58, #ffffff);  /* Background color left to right*/
                color: #000000; /* Text color */
            }
    
            .light-mode .project {
                background-color: #ffffff; /* Background color */
                color: #333f58; /* Text  color */
            }
    
            .light-mode .project h2 {
                color: #333f58; /* Text color */
            }
    
            .light-mode .project h3 {
                color: #333f58; /* Text color */
            }
    
            .light-mode .details{
                color: #666666; /* Text color */
            }
    
            .light-mode .project p {
                color: #666666; /* Text color */
            }
    
            .light-mode footer {
                background: linear-gradient(90deg, #333f58, #ffffff); /* Background color left to right*/
                color: #000000; /* Text color */
            }
    
            .light-mode .project a { 
                background-color: #333f58; /* Background color */
            }
            
            .light-mode .github-button{
                background-color: #333f58; /* Button color on hover */
            }

            .light-mode .github-button:hover{
                background-color: #242d3f; /* Button color on hover */
                transform: scale(1.05); /* Slightly scales up on hover */
            }

            .light-mode .back-to-top-button{
                background-color: #333f58; /* Button color on hover */
            }

            .light-mode .back-to-top-button:hover{
                background-color: #242d3f; /* Button color on hover */
                transform: scale(1.05); /* Slightly scales up on hover */
            }

            .dark-mode-toggle { /* Change Theme icon */
                position: absolute; /*Absolute position, no container*/
                top: 20px; /* 20 pc from the top */
                right: 20px; /* 20 px from the right */
                width: 30px; /* Icon width */
                height: 30px; /* Icon height */
                cursor: pointer; /* Type of cursor*/
                transition: transform 0.3s; /* Animation Timer */
            }
    
            .dark-mode-toggle:hover {
                transform: scale(1.5); /* Scale image */
            }

            footer {
                margin-top: 10px; /* Puts a margin at the top */
                padding: 20px; /* Spacing */
                text-align: center; /* Text Center */
                width: 100%; /* Occupies 100% of the container */
                background: linear-gradient(90deg, #ef8354, #000000); /* Background color left to right*/
                color: #b0c4de; /* Text Color */
                font-size: 0.9em; /* Font Size */
            }
            
            @media (max-width: 768px) { /* Setting for mobile */

                header h1 {
                    font-size: 2.5em;
                }

                header p {
                    font-size: 1.2em;
                }

                .project {
                    flex-direction: column;
                    align-items: center;
                }

                .project img {
                    max-width: 100%;
                }

                .container {
                    padding: 0 10px;
                }

                footer {
                    font-size: 1em;
                }
            }
        </style>
    </head>
    <body class="dark-mode" id="top">
        <header>
            <h1>My Projects</h1>
            <p>Explore my portfolio! Check out my latest projects.</p>
        </header>
        <!-- CV Icon -->
        <a href="img/CV.pdf" target="_blank" >
            <img src="img/Bcontact.png" class="cv-button" id="contactIcon">
        </a>
        <!-- Theme Icon -->
        <img src="img/sun.png" class="dark-mode-toggle" onclick="toggleDarkMode()" id="darkModeIcon">
    
        <div class="container">

             <div class="project"> <!-- Start of a project -->
                <img src="img/image.jpg"> <!-- Project image -->
                <div class="project-content"> <!-- Container for project content -->
                        <h2>Project</h2> <!-- Project title -->
                        <p>Project description</p><!-- Project description -->
                        <a href="https://github.com/gabrielecossutta/VFX/tree/main" target="_blank">Look on GitHub</a>
                </div>
                <div class="details"> <!-- Container for details level -->
        	        <h3>Skills</h3> <!-- Title for details level -->
                    <p>Unreal - Unity</p>
                    <h3>Level of Completion</h3> <!-- Title for details level -->
                    <p>10/10</p>
                </div>
            </div>
        </div>
    
        <footer > <!-- when clicked call the scrollToTop Script -->
            <p><a href="https://github.com/gabrielecossutta" target="_blank" class="github-button">Visit my GitHub</a></p>
            <p class="back-to-top-button" onclick="scrollToTop()" >Back to Top  </p >
        </footer>
    
        <script>
            // change icon from moon to sun
            function toggleDarkMode() { 
    
                // Swith from dark to light mode
                document.body.classList.toggle('light-mode'); 
                document.body.classList.toggle('dark-mode');

                // Change icons
                document.getElementById("darkModeIcon").src = document.body.classList.contains('light-mode') ? "img/moon.png" : "img/sun.png"; 
            }
    
            function scrollToTop() { // Scroll till the top on the site 
                window.scrollTo({top: 0});
            }
    
        </script>
    </body>
</html>
