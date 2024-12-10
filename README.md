<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Akhil Krishnan- Electrical and Electronics Engineering </title>
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

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 4rem 0;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
        }

        .profile {
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        .profile-image {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            border: 5px solid white;
            object-fit: cover;
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
            margin-bottom: 1.5rem;
        }

        .profile h1 {
            font-size: 3rem;
            margin-bottom: 0.5rem;
            font-weight: 700;
        }

        .profile-subtitle {
            font-size: 1.25rem;
            opacity: 0.9;
            font-weight: 300;
        }

        nav {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: transform 0.3s ease;
            position: relative;
        }

        nav a::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 2px;
            bottom: -5px;
            left: 0;
            background-color: white;
            transform: scaleX(0);
            transition: transform 0.3s ease;
        }

        nav a:hover::after {
            transform: scaleX(1);
        }

        .card {
            background: var(--card-background);
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            padding: 2rem;
            margin-bottom: 2rem;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-10px);
        }

        section {
            margin-top: 3rem;
        }

        h2 {
            color: var(--primary-color);
            border-bottom: 3px solid var(--secondary-color);
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
        }

        .publication {
            margin-bottom: 1.5rem;
            border-left: 4px solid var(--secondary-color);
            padding-left: 1rem;
        }

        .publication h3 {
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }

        .publication-meta {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .btn-link {
            display: inline-block;
            background-color: var(--secondary-color);
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            margin-right: 0.5rem;
            transition: background-color 0.3s ease;
        }

        .btn-link:hover {
            background-color: var(--primary-color);
        }

        footer {
            background: var(--primary-color);
            color: white;
            text-align: center;
            padding: 2rem 0;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--secondary-color);
        }

        @media (max-width: 768px) {
            header {
                clip-path: none;
                padding: 2rem 0;
            }

            .profile h1 {
                font-size: 2.5rem;
            }

            nav {
                flex-direction: column;
                align-items: center;
            }

            .publication-meta {
                flex-direction: column;
                align-items: flex-start;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="profile">
                <img src="/api/placeholder/250/250" alt="Dr. Emily Rodriguez" class="profile-image">
                <h1>Dr. Emily Rodriguez</h1>
                <p class="profile-subtitle">PhD Candidate | Computer Vision & Machine Learning</p>
                <p class="profile-subtitle">Stanford University | Human-Centered AI Lab</p>
            </div>
            <nav>
                <a href="#about" aria-label="About section">About</a>
                <a href="#research" aria-label="Research section">Research</a>
                <a href="#publications" aria-label="Publications section">Publications</a>
                <a href="#projects" aria-label="Projects section">Projects</a>
                <a href="#contact" aria-label="Contact section">Contact</a>
            </nav>
        </div>
    </header>

    <main class="container">
        <section id="about" class="card">
            <h2>About Me</h2>
            <p>I'm a PhD candidate in Computer Science at Stanford University, specializing in computer vision and machine learning. My research focuses on developing advanced AI systems that can understand and interpret complex visual scenes with human-like reasoning.</p>
            <p>My work bridges the gap between perception and cognition, aiming to create more interpretable and ethical AI technologies.</p>
        </section>

        <section id="research" class="card">
            <h2>Research Interests</h2>
            <ul>
                <li>3D Scene Understanding</li>
                <li>Visual Reasoning</li>
                <li>Interpretable Machine Learning</li>
                <li>Human-Centered AI</li>
                <li>Ethical AI Development</li>
            </ul>
        </section>

        <section id="publications">
            <h2>Selected Publications</h2>
            <div class="card publication">
                <div class="publication-meta">
                    <div>
                        <h3>Towards Interpretable 3D Scene Reconstruction</h3>
                        <p>Rodriguez, E., Chen, L., & Kumar, S.</p>
                        <p><em>IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2024</em></p>
                    </div>
                    <div>
                        <a href="#" class="btn-link">Paper</a>
                        <a href="#" class="btn-link">Code</a>
                    </div>
                </div>
            </div>
            <!-- More publications can be added here -->
        </section>

        <section id="projects">
            <h2>Featured Projects</h2>
            <div class="card publication">
                <h3>Visual Reasoning Transformer</h3>
                <p>An advanced neural network architecture that combines computer vision and natural language processing to enable more nuanced scene understanding.</p>
                <div class="publication-meta">
                    <div></div>
                    <div>
                        <a href="#" class="btn-link">Project Page</a>
                        <a href="#" class="btn-link">GitHub</a>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="card">
            <h2>Contact</h2>
            <p>Email: emily.rodriguez@stanford.edu</p>
            <div class="social-links">
                <a href="#" aria-label="GitHub Profile">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
                    </svg>
                </a>
                <a href="#" aria-label="LinkedIn Profile">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path>
                        <rect x="2" y="9" width="4" height="12"></rect>
                        <circle cx="4" cy="4" r="2"></circle>
                    </svg>
                </a>
                <a href="#" aria-label="Google Scholar Profile">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M5.242 13.769L0 9.5 12 2l12 7.5-5.242 4.269C17.548 11.249 14.978 9.5 12 9.5c-2.977 0-5.548 1.748-6.758 4.269zM12 10a7.5 7.5 0 1 0 7.5 7.5c0-4.136-3.364-7.5-7.5-7.5z"/>
                    </svg>
                </a>
                <a href="#" aria-label="Twitter Profile">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 14.01-7.496 14.01-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"/>
                    </svg>
                </a>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2024 Dr. Emily Rodriguez. All rights reserved.</p>
        <p>Personal Academic Portfolio | Built with ❤️ in India, CA</p>
    </footer>
</body>
</html>
