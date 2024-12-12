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
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
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
            max-width: 800px;
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

        ul {
            list-style-type: disc;
            margin-left: 1.5rem;
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
            <img src="/api/placeholder/250/250" alt="Akhil Krishnan" class="profile-image">
            <h1>Akhil Krishnan</h1>
            <p>B.Tech in Electrical and Electronics Engineering | Manipal University Jaipur</p>
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
            <p>As a Bachelor's candidate in Electrical and Electronics Engineering at Manipal University Jaipur, I specialize in areas like non-linear dynamics and advanced control systems. My passion lies in bridging theory with practical applications to create impactful innovations in technology.</p>
        </section>

        <section id="research">
            <h2>Research Interests</h2>
            <ul>
                <li>Anti-Control of Chaos</li>
                <li>Non-Linear Dynamics</li>
                <li>Control Systems</li>
                <li>Ethical AI and Machine Learning</li>
            </ul>
        </section>

        <section id="publications">
            <h2>Publications</h2>
            <p><strong>Title:</strong> "Optimization in Electrical Grids"<br>
            <strong>Journal:</strong> International Journal of Electrical Engineering<br>
            <a href="#" class="btn">Read More</a></p>
        </section>

        <section id="projects">
            <h2>Projects</h2>
            <p>Project: "Smart Grid Solutions"<br>
            <a href="#" class="btn">GitHub Repository</a></p>
        </section>

        <section id="contact">
            <h2>Contact</h2>
            <p>Email: akhil.krishnan@domain.com</p>
        </section>
    </main>
    <footer>
        <p>© 2024 Akhil Krishnan. All rights reserved.</p>
    </footer>
</body>
</html>
