%%<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Akhil Krishnan - Electrical and Electronics Engineering</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
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

        .social-links {
            margin-top: 1.5rem;
            display: flex;
            justify-content: center;
            gap: 1rem;
        }

        .social-links a {
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 1rem;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            background: var(--secondary-color);
            transition: background 0.3s ease;
        }

        .social-links a i {
            font-size: 1.2rem;
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

        .item {
            margin-bottom: 1.5rem;
            border-left: 4px solid var(--secondary-color);
            padding-left: 1rem;
        }

        .item h3 {
            font-size: 1.25rem;
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }

        .item-meta {
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

        footer .contact-info {
            color: white;
        }

        footer .contact-info a {
            color: #26d0ce;
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <div class="profile">
            <img src="profile-photo.jpg" alt="Akhil Krishnan" class="profile-image">
            <h1>Akhil Krishnan</h1>
            <p>B.Tech in Electrical and Electronics Engineering | Manipal University Jaipur</p>
            <div class="social-links">
                <a href="https://www.linkedin.com/in/akhilkrishnan" target="_blank">
                    <i class="fab fa-linkedin"></i> LinkedIn
                </a>
                <a href="https://www.researchgate.net/profile/Akhil-Krishnan" target="_blank">
                    <i class="fas fa-flask"></i> ResearchGate
                </a>
                <a href="https://scholar.google.com/citations?user=XXXXX" target="_blank">
                    <i class="fas fa-graduation-cap"></i> Google Scholar
                </a>
            </div>
        </div>
        <nav>
            <a href="#about">About</a>
            <a href="#special-skills">Special Skills</a>
            <a href="#scholastic-accolades">Accolades</a>
            <a href="#fellowships">Fellowships & Grants</a>
            <a href="#publications">Publications</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <main>
        <section id="about">
            <h2>About Me</h2>
            <p>I am an aspiring engineer passionate about Electrical and Electronics Engineering. With a strong academic foundation from Manipal University Jaipur, I am focused on research and innovative projects.</p>
        </section>
        <section id="special-skills">
            <h2>Special Skills</h2>
            <p>Below are some of the certifications I have earned:</p>
            <div class="item">
                <h3>Skill Name</h3>
                <a href="https://example.com/certification" target="_blank" class="btn">View Certification</a>
            </div>
        </section>
        <section id="scholastic-accolades">
            <h2>Scholastic Accolades</h2>
            <div class="item">
                <h3>Title of Award</h3>
                <p>Description of the award.</p>
                <a href="https://example.com/accolade" target="_blank" class="btn">Learn More</a>
            </div>
        </section>
        <section id="fellowships">
            <h2>Fellowships & Grants</h2>
            <div class="item">
                <h3>State Bank of India, Youth for India </h3>
                Accepted 1 of 76 successful candidates from 50,000 globally,

with a grant intake rate of 0.152%. Received INR 3,07,556.5 ($ 4,335) in emoluments which includes travel

allowance, housing allowance, language training, project allowance & emergency allowance. </p>
                <a href="https://example.com/grant-details" target="_blank" class="btn">Read More</a>
            </div>
        </section>
        <section id="publications">
            <h2>Publications</h2>
            <div class="item">
                <h3>Non-linear Dynamical Analysis of an Inverted Pendulum Cart Mechanism using Bifurcation Method</h3>
                <p>Published in: IEEE, 2019</p>
                <a href="https://ieeexplore.ieee.org/document/8993310" target="_blank" class="btn">Read Paper</a>
                <a href="https://github.com/akhilkrishnan/research-code" target="_blank" class="btn">View Code</a>
            </div>
            <div class="item">
            <h3>A Comparative Study on Intelligent & Adaptive Control Techniques on a Nonlinear Inverted Pendulum Cart Mechanism </h3>
                <p>Published in: IEEE, 2021</p>
                <a href="https://ieeexplore.ieee.org/document/9596243" target="_blank" class="btn">Read Paper</a>
                <a href="https://github.com/akhilkrishnan/research-code" target="_blank" class="btn">View Code</a>
            </div>
            <div class="item">
<h3>Desalination of Marine water using Machine Learning Methods</h3>
                <p>Published in: IEEE, 2021</p>
                <a href="https://ieeexplore.ieee.org/document/9596489" target="_blank" class="btn">Read Paper</a>
                <a href="https://github.com/akhilkrishnan/research-code" target="_blank" class="btn">View Code</a>
            </div> 
        </section>
        <section id="projects">
            <h2>Projects</h2>
            <div class="item">
                <h3>Project Title</h3>
                <p>Brief description of the project.</p>
                <a href="https://example.com/project" target="_blank" class="btn">View Project</a>
                <a href="https://github.com/akhilkrishnan/project-code" target="_blank" class="btn">View Code</a>
            </div>
        </section>
        <section id="contact">
            <h2>Contact</h2>
            <p>Email: <a href="mailto:akhil.krishnan@domain.com">akhil.krishnan@domain.com</a></p>
            <p>Phone: +91-12345-67890</p>
        </section>
    </main>
    <footer>
        <p>© 2024 Akhil Krishnan. All rights reserved.</p>
    </footer>
</body>
</html>
