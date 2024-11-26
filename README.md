<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Science Portfolio</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/typed.js/2.0.12/typed.min.js"></script>
    <style>
        :root {
            --primary-color: #2563eb;
            --secondary-color: #1e40af;
            --text-color: #1f2937;
            --bg-color: #ffffff;
            --section-bg: #f3f4f6;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        }

        body {
            line-height: 1.6;
            color: var(--text-color);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--bg-color);
            padding: 20px 0;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary-color);
        }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary-color);
        }

        /* Hero Section */
        .hero {
            padding: 160px 0 100px;
            background-color: var(--bg-color);
            text-align: center;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            color: var(--text-color);
        }

        .hero p {
            font-size: 20px;
            color: #4b5563;
            margin-bottom: 30px;
        }

        .typed-text {
            color: var(--primary-color);
        }

        /* About Section */
        .about {
            padding: 100px 0;
            background-color: var(--section-bg);
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-text h2 {
            font-size: 36px;
            margin-bottom: 20px;
        }

        .about-text p {
            margin-bottom: 20px;
        }

        /* Skills Section */
        .skills {
            padding: 100px 0;
            background-color: var(--bg-color);
        }

        .skills h2 {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .skill-card {
            background-color: var(--section-bg);
            padding: 30px;
            border-radius: 10px;
            text-align: center;
        }

        .skill-card h3 {
            margin: 20px 0;
        }

        /* Projects Section */
        .projects {
            padding: 100px 0;
            background-color: var(--section-bg);
        }

        .projects h2 {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .project-card {
            background-color: var(--bg-color);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .project-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .project-content {
            padding: 20px;
        }

        .project-content h3 {
            margin-bottom: 10px;
        }

        /* Contact Section */
        .contact {
            padding: 100px 0;
            background-color: var(--bg-color);
            text-align: center;
        }

        .contact h2 {
            font-size: 36px;
            margin-bottom: 50px;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 50px;
            margin-bottom: 50px;
        }

        .contact-item {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* Footer */
        footer {
            background-color: var(--text-color);
            color: var(--bg-color);
            padding: 20px 0;
            text-align: center;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .contact-info {
                flex-direction: column;
                gap: 30px;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">Portfolio</div>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#skills">Skills</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Hello, I'm <span class="typed-text"></span></h1>
            <p>Information Systems Graduate | Data Science Enthusiast</p>
        </div>
    </section>

    <section id="about" class="about">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>About Me</h2>
                    <p>I am an Information Systems graduate with a passion for data science and analytics. My academic background combines technical expertise with business acumen, allowing me to transform complex data into actionable insights.</p>
                    <p>Currently focusing on developing my skills in machine learning, statistical analysis, and data visualization while pursuing projects that make a real-world impact.</p>
                </div>
                <div class="about-image">
                    <img src="/api/placeholder/500/500" alt="Profile Picture" style="width: 100%; border-radius: 10px;">
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="skills">
        <div class="container">
            <h2>Technical Skills</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <h3>Data Analysis</h3>
                    <p>Python, R, SQL, Excel</p>
                </div>
                <div class="skill-card">
                    <h3>Machine Learning</h3>
                    <p>Scikit-learn, TensorFlow, Neural Networks</p>
                </div>
                <div class="skill-card">
                    <h3>Visualization</h3>
                    <p>Tableau, Power BI, Matplotlib, Seaborn</p>
                </div>
                <div class="skill-card">
                    <h3>Tools & Technologies</h3>
                    <p>Git, Jupyter, AWS, Docker</p>
                </div>
            </div>
        </div>
    </section>

    <section id="projects" class="projects">
        <div class="container">
            <h2>Featured Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <img src="/api/placeholder/400/200" alt="Project 1">
                    <div class="project-content">
                        <h3>Data Analysis Project</h3>
                        <p>Analysis of customer behavior using Python and SQL.</p>
                    </div>
                </div>
                <div class="project-card">
                    <img src="/api/placeholder/400/200" alt="Project 2">
                    <div class="project-content">
                        <h3>Machine Learning Model</h3>
                        <p>Predictive model for market trends using TensorFlow.</p>
                    </div>
                </div>
                <div class="project-card">
                    <img src="/api/placeholder/400/200" alt="Project 3">
                    <div class="project-content">
                        <h3>Dashboard Development</h3>
                        <p>Interactive dashboard using Tableau and Power BI.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2>Get In Touch</h2>
            <div class="contact-info">
                <div class="contact-item">
                    <h3>Email</h3>
                    <p>your.email@example.com</p>
                </div>
                <div class="contact-item">
                    <h3>LinkedIn</h3>
                    <p>linkedin.com/in/yourprofile</p>
                </div>
                <div class="contact-item">
                    <h3>GitHub</h3>
                    <p>github.com/yourusername</p>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Your Name. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Typing animation
        new Typed('.typed-text', {
            strings: ['a Data Scientist', 'an Analyst', 'a Problem Solver'],
            typeSpeed: 100,
            backSpeed: 50,
            loop: true
        });
    </script>
</body>
</html>
