<!DOCTYPE html>
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
            width: 200px;
            height: 200px;
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
                <h3>TRIZ Level-1 </h3>
                <a href="https://example.com/certification" target="_blank" class="btn">View Certification</a>
            </div>
        </section>
        <section id="scholastic-accolades">
            <h2>Scholastic Accolades</h2>
            <div class="item">
                <h3>Summa Cum Laude</h3>
                <p>Awarded Summa Cum Laude with a Grade Point Average (GPA) of 10/10 in the eighth semester of Engineering</p>
                <a href="https://tinyurl.com/49tbb37a" target="_blank" class="btn">View Certification</a>
            </div>
            <div class="item">
                 <h3>Top 1% out of 358 students</h3>
                <p>Awarded with A+ grade in 7 different subjects such as switch gears and protection,
communication systems, power system operation and control, flexible AC transmission system, linear control
systems, Bioinformatics for Engineers and sustainable development courses for exceptional performance.</p>
            </div>
       </section>
        <section id="fellowships">
            <h2>Fellowships & Grants</h2>
            <div class="item">
                <h3>State Bank of India - Youth for India Fellowship</h3>
            <p>Accepted 1 of 76 successful candidates from 50,000 globally, with a grant intake rate of 0.152%. Received INR 3,07,556.5 ($ 4,335) in emoluments which includes travel allowance, housing allowance, language training, project allowance & emergency allowance.</p>
                <a href="https://example.com/grant-details" target="_blank" class="btn">Read More</a>
            </div>
            <div class="item">
            <h3>Global Digital Corps Field Ops Fellowship</h3> 
 <p>At time of a national emergency, the certificate holder has a basic
understanding of disaster management and field operations and can be a valuable volunteer for the benefit of
the society.</p>
    <a href="https://example.com/grant-details" target="_blank" class="btn">Read More</a>
            </div>
<div class="item">
<h3>Manipal University Research Grant</h3> 
<p>Received sum of INR 15,162 ($ 227.43) as a financial aid for presenting
research paper on Nonlinear Dynamics at an International Conference conducted by IEEE. The fund included
circumnavigation, registration fee & other expenses.</p>
<a href="https://example.com/grant-details" target="_blank" class="btn">Read More</a>
</div>
            <div class="item">
    <h3>Rajasthan Administrative Service Grants </h3>
   <p>Received sum of INR 30,000 for the Installation of RO plant in theproject VASUDHA: The Lifeblood of Rural Communities.</p>
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
                <h3>A Comparative Study on Intelligent & Adaptive Control Techniques on a Nonlinear Inverted Pendulum Cart Mechanism</h3>
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
            <h2> Projects : Technology for Social Impact</h2>
            <div class="item">
                <h2>VASUDHA : The Lifeblood of Rural Communities</h2>
                <section class="project-overview">
                    <h3>Project Description :</h3>
                    <p>VASUDHA stands for <em>Village And School Underpin by providing Safe and clean drinking water for Health Amelioration in the community via Technological Intervention</em></p>
                </section>
                <section class="project-summary">
                    <h3>Project Summary :</h3>
                    <p>In a transformative rural development project, a strategically positioned Reverse Osmosis (RO) plant now provides 1,200 liters of clean drinking water daily, directly benefiting 400+ rural residents and a school across the target community. The initiative demonstrates addressing critical drinking water challenges through an innovative and holistic approach.</p>
  <p>The project distinguished itself through a unique blend of technological innovation and cultural sensitivity, securing robust community engagement. By establishing a Village Water Committee and conducting extensive training programs, the initiative fostered local ownership and capacity building. Specifically, the team educated 260+ community members through interactive puppetry workshops, trained 5 healthcare workers on water-related health risks, and achieved 100% local leadership transition within just 10 months.</p>
 <p>Financial stewardship was a critical component of the project's success. With a strategic budget management approach, effectively handled INR 81,760, strategically sourcing materials from within the village to reduce costs by 10%. Additionally, a catalytic government grant of INR 30,000 was secured, further amplifying the project's impact and sustainability.</p>
<p>An innovative solution to wastewater disposal was implemented using Aloe vera-inspired phytoremediation techniques. This approach not only addressed environmental concerns but also demonstrated a sophisticated understanding of integrated water management, creating a comprehensive system for water purification, wastewater treatment, and groundwater conservation.</p>
                    <p>The long-term sustainability of the project is ensured through the establishment of a dedicated maintenance fund managed via a post office account and overseen by the Village Water Committee. By bridging micro and macro developmental gaps, this initiative promises generational benefits, setting a scalable model for rural water infrastructure that can be replicated across multiple villages.</p>
<p>Ultimately, the project exemplifies a nuanced, holistic approach to rural development—one that respects local traditions, leverages technological solutions, and empowers communities to take charge of their critical infrastructure and health outcomes.</p>
                    <div class="project-links">
                        <a href="https://example.com/project" target="_blank" class="btn">View Project</a>
                        <a href="https://github.com/akhilkrishnan/project-code" target="_blank" class="btn">View Source Code</a>
                        <a href="https://mega.nz/file/Z3Z1DAbD#DljdHC-U0nu5R2DYb6a05oA17I0sL21xWAoMatlvDVU" target="_blank" class="btn">View Press Releases - PDF</a>
                    </div>
                </section>
            </div>
        </section>
<section id="contact">
            <h2>Contact</h2>
            <div class="contact-info">
                <p>Email: <a href="mailto:akhil.krishnan@domain.com">akhil.krishnan@domain.com</a></p>
                <p>Phone: +91-12345-67890</p>
            </div>
        </section>
      
   </main>
    <footer>
        <p>© 2024 Akhil Krishnan. All rights reserved.</p>
        <p>Personal Academic Portfolio | Built with ❤️ in India</p>
    </footer>
</body>
</html>
