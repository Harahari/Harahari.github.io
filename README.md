# Harahari.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Academic Portfolio</title>
    <style>
        :root {
            --bg-color: #ffffff;
            --text-color: #2d3436;
            --accent-color: #0984e3;
            --gray-light: #dfe6e9;
            --gray-dark: #636e72;
            --spacing-unit: 8px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background: var(--bg-color);
            font-size: 16px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: calc(var(--spacing-unit) * 4);
        }

        /* Typography */
        h1, h2, h3 {
            font-weight: 700;
            line-height: 1.2;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: calc(var(--spacing-unit) * 3);
        }

        h2 {
            font-size: 1.75rem;
            margin: calc(var(--spacing-unit) * 6) 0 calc(var(--spacing-unit) * 3);
        }

        h3 {
            font-size: 1.25rem;
            margin: calc(var(--spacing-unit) * 3) 0 var(--spacing-unit);
        }

        p {
            margin-bottom: calc(var(--spacing-unit) * 2);
        }

        /* Header Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: calc(var(--spacing-unit) * 4) 0;
            position: relative;
        }

        .profile-info {
            animation: fadeIn 1s ease-out;
        }

        .title {
            font-size: 1.25rem;
            color: var(--gray-dark);
            margin-bottom: calc(var(--spacing-unit) * 4);
        }

        .bio {
            font-size: 1.1rem;
            max-width: 600px;
            margin-bottom: calc(var(--spacing-unit) * 4);
        }

        /* Navigation */
        .nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: calc(var(--spacing-unit) * 2) 0;
            transition: transform 0.3s ease;
        }

        .nav.hidden {
            transform: translateY(-100%);
        }

        .nav-container {
            max-width: 800px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 calc(var(--spacing-unit) * 4);
        }

        .nav-links a {
            margin-left: calc(var(--spacing-unit) * 3);
            text-decoration: none;
            color: var(--text-color);
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent-color);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        /* Publications */
        .publication-item {
            margin-bottom: calc(var(--spacing-unit) * 4);
            padding: calc(var(--spacing-unit) * 3);
            border: 1px solid var(--gray-light);
            border-radius: 8px;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .publication-item:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .publication-title {
            color: var(--accent-color);
            margin-bottom: var(--spacing-unit);
        }

        .authors {
            color: var(--gray-dark);
            margin-bottom: var(--spacing-unit);
        }

        .venue {
            font-style: italic;
            color: var(--gray-dark);
            margin-bottom: calc(var(--spacing-unit) * 2);
        }

        .links {
            display: flex;
            gap: calc(var(--spacing-unit) * 2);
        }

        .links a {
            text-decoration: none;
            color: var(--accent-color);
            padding: 6px 12px;
            border: 1px solid var(--accent-color);
            border-radius: 4px;
            font-size: 0.9rem;
            transition: all 0.2s ease;
        }

        .links a:hover {
            background: var(--accent-color);
            color: white;
        }

        /* Projects */
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: calc(var(--spacing-unit) * 3);
            margin-top: calc(var(--spacing-unit) * 3);
        }

        .project-card {
            border: 1px solid var(--gray-light);
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .project-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .project-image {
            width: 100%;
            height: 160px;
            background: var(--gray-light);
            object-fit: cover;
        }

        .project-info {
            padding: calc(var(--spacing-unit) * 2);
        }

        /* Contact */
        .contact-section {
            margin-top: calc(var(--spacing-unit) * 8);
            text-align: center;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: calc(var(--spacing-unit) * 3);
            margin-top: calc(var(--spacing-unit) * 3);
        }

        .social-links a {
            color: var(--gray-dark);
            text-decoration: none;
            transition: color 0.2s ease;
        }

        .social-links a:hover {
            color: var(--accent-color);
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 768px) {
            .container {
                padding: calc(var(--spacing-unit) * 2);
            }

            .hero {
                min-height: auto;
                padding: calc(var(--spacing-unit) * 8) 0;
            }

            .nav-links {
                display: none;
            }

            .project-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <nav class="nav">
        <div class="nav-container">
            <div class="logo">YN</div>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#publications">Publications</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </div>
        </div>
    </nav>

    <div class="container">
        <section class="hero">
            <div class="profile-info">
                <h1>Your Name</h1>
                <div class="title">PhD Student in Computer Science</div>
                <p class="bio">
                    I'm a computer science researcher at University Name, focusing on computer vision 
                    and machine learning. My work explores the intersection of 3D scene understanding 
                    and visual reasoning.
                </p>
                <div class="links">
                    <a href="#publications">View Publications</a>
                    <a href="#contact">Get in Touch</a>
                </div>
            </div>
        </section>

        <section id="publications">
            <h2>Selected Publications</h2>
            <div class="publication-item">
                <h3 class="publication-title">Paper Title: A Novel Approach to Something Interesting</h3>
                <div class="authors">Your Name, Coauthor One, Coauthor Two</div>
                <div class="venue">CVPR 2024</div>
                <div class="links">
                    <a href="#">Paper</a>
                    <a href="#">Code</a>
                    <a href="#">Project</a>
                    <a href="#">Blog</a>
                </div>
            </div>
            <!-- More publications -->
        </section>

        <section id="projects">
            <h2>Featured Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <img src="/api/placeholder/400/320" alt="Project 1" class="project-image">
                    <div class="project-info">
                        <h3>Project Name</h3>
                        <p>Brief description of the project and its key findings or impact.</p>
                        <div class="links">
                            <a href="#">Demo</a>
                            <a href="#">Code</a>
                        </div>
                    </div>
                </div>
                <!-- More projects -->
            </div>
        </section>

        <section id="contact" class="contact-section">
            <h2>Get in Touch</h2>
            <p>Feel free to reach out for collaborations or questions.</p>
            <p>email@university.edu</p>
            <div class="social-links">
                <a href="#">GitHub</a>
                <a href="#">Twitter</a>
                <a href="#">LinkedIn</a>
                <a href="#">Scholar</a>
            </div>
        </section>
    </div>

    <script>
        // Smooth scroll for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Hide navbar on scroll down, show on scroll up
        let lastScroll = 0;
        const navbar = document.querySelector('.nav');

        window.addEventListener('scroll', () => {
            const currentScroll = window.pageYOffset;
            if (currentScroll <= 0) {
                navbar.classList.remove('hidden');
                return;
            }
            
            if (currentScroll > lastScroll && !navbar.classList.contains('hidden')) {
                navbar.classList.add('hidden');
            } else if (currentScroll < lastScroll && navbar.classList.contains('hidden')) {
                navbar.classList.remove('hidden');
            }
            lastScroll = currentScroll;
        });
    </script>
</body>
</html>
