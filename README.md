<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Akhil Krishnan - Electrical and Electronics Engineering</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #1a2980;
            --secondary-color: #26d0ce;
            --text-color: #2c3e50;
            --background-color: #f4f7f6;
            --card-background: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.7;
            color: var(--text-color);
            background-color: var(--background-color);
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 3rem 0;
            text-align: center;
        }

        .profile-image {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            margin: 0 auto 1rem;
            border: 4px solid white;
        }

        .profile h1 {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        .profile p {
            font-size: 1rem;
            opacity: 0.85;
        }

        .contact-info {
            margin: 1rem 0;
        }

        .contact-info p {
            font-size: 1rem;
            margin: 0.5rem 0;
        }

        .social-links {
            margin-top: 1rem;
        }

        .social-links a {
            color: white;
            text-decoration: none;
            margin: 0 0.5rem;
            font-size: 1.2rem;
            display: inline-block;
            padding: 0.5rem 0.75rem;
            border-radius: 5px;
            background: var(--secondary-color);
            transition: background 0.3s ease;
        }

        .social-links a:hover {
            background: var(--primary-color);
        }

        nav {
            margin-top: 1.5rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 1rem;
            font-size: 1rem;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: var(--secondary-color);
        }

        main {
            margin: 2rem auto;
            max-width: 900px;
            padding: 0 1rem;
        }

        section {
            margin-bottom: 2rem;
            background: var(--card-background);
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
            padding: 1.5rem;
        }

        section h2 {
            color: var(--primary-color);
            font-size: 1.5rem;
            border-bottom: 2px solid var(--secondary-color);
            padding-bottom: 0.5rem;
            margin-bottom: 1rem;
        }

        .publication {
            margin-bottom: 1.5rem;
            border-left: 4px solid var(--secondary-color);
            padding-left: 1rem;
        }

        .publication h3 {
            font-size: 1.25rem;
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }

        .publication-meta {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 0.5rem 1rem;
            margin-top: 0.5rem;
            color: white;
            background: var(--primary-color);
            text-decoration: none;
            border-radius: 5px;
            font-size: 0.9rem;
        }

        .btn:hover {
            background: var(--secondary-color);
        }

        footer {
            text-align: center;
            padding: 1rem 0;
            background: var(--primary-color);
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <div class="profile">
            <img src="profile-photo.jpg" alt="Akhil Krishnan" class="profile-image">
            <h1>Akhil Krishnan</h1>
            <p>B.Tech in Electrical and Electronics Engineering | Manipal University Jaipur</p>
            <div class="contact-info">
                <p>Email: <a href="mailto:akhil.krishnan@domain.com" style="color: white; text-decoration: underline;">akhil.krishnan@domain.com</a></p>
                <p>Phone: +91-12345-67890</p>
            </div>
            <div class="social-links">
                <a href="https://www.linkedin.com/in/akhilkrishnan" target="_blank">LinkedIn</a>
                <a href="https://www.researchgate.net/profile/Akhil-Krishnan" target="_blank">ResearchGate</a>
                <a href="https://scholar.google.com/citations?user=XXXXX" target="_blank">Google Scholar</a>
            </div>
        </div>
        <nav>
            <a href="#about">About</a>
            <a href="#research">Research</a>
            <a href="#publications">Publications</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <main>
        <section id="about">
            <h2>About Me</h2>
            <p>I am a Bachelor's candidate specializing in Electrical and Electronics Engineering at Manipal University Jaipur. My academic focus lies in Non-Linear Dynamics and advanced control systems. I aim to combine technical skills with innovative approaches to solve modern engineering challenges.</p>
        </section>

        <section id="research">
            <h2>Research Interests</h2>
            <ul>
                <li>Anti-Control of Chaos</li>
                <li>Non-Linear Dynamics</li>
                <li>Ethical AI Systems</li>
                <li>Energy Management in Smart Grids</li>
            </ul>
        </section>

        <section id="publications">
            <h2>Publications</h2>
            <div class="publication">
                <h3>Optimization in Electrical Grids</h3>
                <p><strong>Journal:</strong> International Journal of Electrical Engineering</p>
                <div class="publication-meta">
                    <a href="https://link-to-paper.com" class="btn">Read Paper</a>
                    <a href="https://github.com/akhilkrishnan/paper-code" class="btn">Code</a>
                </div>
            </div>
        </section>

        <section id="projects">
            <h2>Projects</h2>
            <div class="publication">
                <h3>Smart Grid Solutions</h3>
                <p>Developed a solution to optimize energy usage in smart grids using non-linear control theories.</p>
                <div class="publication-meta">
                    <a href="https://link-to-project.com" class="btn">Project Page</a>
                    <a href="https://github.com/akhilkrishnan/smart-grid" class="btn">GitHub</a>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2>Contact</h2>
            <p>Email: akhil.krishnan@domain.com</p>
            <p>Feel free to reach out for collaborations or research inquiries!</p>
        </section>
    </main>
    <footer>
        <p>© 2024 Akhil Krishnan. All rights reserved.</p>
    </footer>
</body>
</html>
