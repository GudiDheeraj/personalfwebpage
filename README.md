Project Name

A modern, responsive web page template with a clean design. It features a navigation bar, sections for featured content, an about page, project showcases, a contact form, and a footer. The design utilizes custom CSS and Unicons for icons.

Table of Contents

Introduction

Installation

Usage

File Structure

Detailed Code Explanation

HTML

CSS

Customization

Colors

Fonts

Images

Contributing

Introduction

This project is a template for a modern web page designed to be clean, simple, and responsive. It includes:

A responsive navigation bar with logo and menu items
A hero section with a background image and overlay text
An about section with text content
A projects section showcasing different works
A contact section with a form
A footer with social media icons
Installation
To get a local copy up and running, follow these steps.

Prerequisites
A web browser (e.g., Chrome, Firefox, Edge)
Text editor (e.g., VSCode, Sublime Text)
Git
Clone the Repository
Open your terminal.
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/your-repository-name.git
Navigate to the project directory:
bash
Copy code
cd your-repository-name
Open the HTML File
Open the index.htm file in your preferred web browser to view the project.

Usage
This section describes how to use the project, how to navigate through different sections, and any interactive features.

Navigating the Website
Navigation Bar: Use the navigation bar to quickly jump to different sections of the page.
Hero Section: The landing section with an eye-catching background image and welcome text.
About Section: Learn more about the purpose or the team behind the project.
Projects Section: View showcases of various projects with descriptions and links.
Contact Section: Fill out and submit the contact form to get in touch.
Footer: Find social media links and other pertinent information.
File Structure
Copy code
your-repository-name/
├── cswam.png
├── csww.png
├── dheeraj.jpg
├── gcp2.png
├── gcp.png
├── index.htm
└── README.md
index.htm
This is the main HTML file containing the structure of the web page. It includes sections like the navigation bar, featured content, about section, projects, and contact form.

Detailed Code Explanation
HTML
The index.htm file is structured as follows:

html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Modern web page template">
    <title>Project Name</title>
    <link rel="stylesheet" href="assets/css/styles.css">
    <link rel="icon" type="image/png" href="assets/images/favicon.png">
</head>
<body>
    <!-- Navigation -->
    <header class="header" id="header">
        <nav class="nav container">
            <a href="#" class="nav__logo">LOGO</a>
            <div class="nav__menu" id="nav-menu">
                <ul class="nav__list">
                    <li class="nav__item"><a href="#home" class="nav__link active-link">Home</a></li>
                    <li class="nav__item"><a href="#about" class="nav__link">About</a></li>
                    <li class="nav__item"><a href="#projects" class="nav__link">Projects</a></li>
                    <li class="nav__item"><a href="#contact" class="nav__link">Contact</a></li>
                </ul>
                <div class="nav__close" id="nav-close"><i class="uil uil-times"></i></div>
            </div>
            <div class="nav__toggle" id="nav-toggle"><i class="uil uil-apps"></i></div>
        </nav>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Home Section -->
        <section class="home" id="home">
            <div class="home__container container grid">
                <div class="home__content">
                    <h1 class="home__title">Welcome to Our Website</h1>
                    <p class="home__description">This is a modern web page template designed with custom CSS and responsive design principles.</p>
                    <a href="#about" class="button">Learn More</a>
                </div>
                <img src="assets/images/home-image.jpg" alt="Welcome Image" class="home__img">
            </div>
        </section>

        <!-- About Section -->
        <section class="about section" id="about">
            <h2 class="section__title">About Us</h2>
            <div class="about__container container grid">
                <div class="about__data">
                    <p class="about__description">This section provides information about the purpose or the team behind the project.</p>
                </div>
                <img src="assets/images/about-image.jpg" alt="About Image" class="about__img">
            </div>
        </section>

        <!-- Projects Section -->
        <section class="projects section" id="projects">
            <h2 class="section__title">Our Projects</h2>
            <div class="projects__container container grid">
                <div class="project__content">
                    <h3 class="project__title">Project Title 1</h3>
                    <p class="project__description">Brief description of the project.</p>
                </div>
                <div class="project__content">
                    <h3 class="project__title">Project Title 2</h3>
                    <p class="project__description">Brief description of the project.</p>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section class="contact section" id="contact">
            <h2 class="section__title">Contact Us</h2>
            <div class="contact__container container grid">
                <form action="#" class="contact__form">
                    <div class="contact__inputs">
                        <input type="text" placeholder="Name" class="contact__input">
                        <input type="email" placeholder="Email" class="contact__input">
                    </div>
                    <textarea placeholder="Message" class="contact__input"></textarea>
                    <button type="submit" class="button">Send Message</button>
                </form>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer__container container">
            <h1 class="footer__title">LOGO</h1>
            <ul class="footer__list">
                <li><a href="#" class="footer__link">Home</a></li>
                <li><a href="#about" class="footer__link">About</a></li>
                <li><a href="#projects" class="footer__link">Projects</a></li>
                <li><a href="#contact" class="footer__link">Contact</a></li>
            </ul>
            <div class="footer__social">
                <a href="#" class="footer__social-link"><i class="uil uil-facebook-f"></i></a>
                <a href="#" class="footer__social-link"><i class="uil uil-twitter"></i></a>
                <a href="#" class="footer__social-link"><i class="uil uil-instagram"></i></a>
            </div>
        </div>
    </footer>

    <!-- Scroll Up -->
    <a href="#" class="scrollup" id="scroll-up"><i class="uil uil-arrow-up"></i></a>

    <!-- JavaScript -->
    <script src="assets/js/main.js"></script>
</body>
</html>
CSS
The styles.css file contains the styles for the web page. Here is an overview of some key parts:

Variables
Define color variables for easy customization:

css
Copy code
:root {
    --body-color: #000; /* Black background */
    --text-color-primary: #fff; /* White for primary text */
    --text-color-secondary: #ccc; /* Light grey for secondary text */
    --deep-blue: #00008b; /* Deep blue color */
    --first-color: #6b57e0; /* Purple */
    --first-color-hover: #285bd4; /* Darker purple on hover */
    --big-color: #87CEEB; /* Sky blue */
    --big-color-hover: #fff; /* White on hover */
    --second-color: #00c9ff; /* Light blue */
    --third-color: #c0a631; /* Gold */
    --first-shadow-color: rgba(255, 255, 255, 0.2); /* Softer shadow color */
}
Global Styles
Set global styles for the body and text:

css
Copy code
body {
    font-family: 'Poppins', sans-serif;
    background-color: var(--body-color);
    color: var(--text-color-primary);
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

h1, h2, h3, h4, h5, h6 {
    margin: 0;
    color: var(--text-color-primary);
}
Header and Navigation
Styles for the navigation bar:

css
Copy code
.header {
    width: 100%;
    height: 60px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    background-color: var(--body-color);
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1000;
}

.nav {
    display: flex;
    align-items: center;
}

.nav__logo {
    font-size: 1.5rem;
    font-weight: 600;
    color: var(--text-color-primary);
    text-decoration: none;
}

.nav__menu {
    display: flex;
    align-items: center;
    gap: 1.5rem;
}

.nav__link {
    color: var(--text-color-primary);
    text-decoration: none;
    font-size: 1rem;
    transition: 0.3s;
}

.nav__link:hover, .nav__link.active-link {
    color: var(--first-color);
}

.nav__toggle, .nav__close {
    display: none;
    font-size: 1.5rem;
    cursor: pointer;
}
Hero Section
Styles for the hero section:

css
Copy code
.home {
    display: flex;
    align-items: center;
    justify-content: center;
    background: url('home-image.jpg') no-repeat center center/cover;
    height: 100vh;
    color: var(--text-color-primary);
    text-align: center;
}

.home__container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1rem;
}

.home__title {
    font-size: 3rem;
    font-weight: 700;
}

.home__description {
    font-size: 1.25rem;
    margin-bottom: 2rem;
}

.button {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    background-color: var(--first-color);
    color: var(--text-color-primary);
    border-radius: 0.5rem;
    text-decoration: none;
    transition: 0.3s;
}

.button:hover {
    background-color: var(--first-color-hover);
}
Responsive Design
Responsive styles for mobile devices:

css
Copy code
@media screen and (max-width: 768px) {
    .header {
        flex-direction: column;
        height: auto;
        padding: 1rem;
    }

    .nav__menu {
        flex-direction: column;
        align-items: center;
        gap: 1rem;
    }

    .home {
        height: auto;
        padding: 2rem;
    }

    .home__title {
        font-size: 2rem;
    }

    .home__description {
        font-size: 1rem;
    }

    .about__container, .projects__container, .contact__container {
        flex-direction: column;
        align-items: center;
    }

    .about__img, .projects__img, .contact__img {
        width: 100%;
    }
}
Customization
Colors
To customize the colors used in the project, modify the variables defined in the :root selector in the styles.css file.

css
Copy code
:root {
    --body-color: #000; /* Black background */
    --text-color-primary: #fff; /* White for primary text */
    --text-color-secondary: #ccc; /* Light grey for secondary text */
    --deep-blue: #00008b; /* Deep blue color */
    --first-color: #6b57e0; /* Purple */
    --first-color-hover: #285bd4; /* Darker purple on hover */
    --big-color: #87CEEB; /* Sky blue */
    --big-color-hover: #fff; /* White on hover */
    --second-color: #00c9ff; /* Light blue */
    --third-color: #c0a631; /* Gold */
    --first-shadow-color: rgba(255, 255, 255, 0.2); /* Softer shadow color */
}
Fonts
The project uses the Poppins font. You can change the font by modifying the @import statement in the styles.css file.

css
Copy code
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');
Images
Replace the images in the root directory with your own images. Update the img tags in the index.htm file accordingly.



