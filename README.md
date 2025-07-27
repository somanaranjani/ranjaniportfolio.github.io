<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Somana Siva Ranjani - Quality Assurance & BI Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            transition: all 0.3s ease;
        }

        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.5rem 0;
            width: 100%;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: white;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
            position: absolute;
            left: 20px;
            top: 50%;
            transform: translateY(-50%);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
            margin-left: auto;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
            margin-left: auto;
        }

        .nav-links a {
            text-decoration: none;
            color: white;
            font-weight: 500;
            transition: color 0.3s ease;
            text-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
        }

        .nav-links a:hover {
            color: #f0f0f0;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
        }

        /* Hero Section */
        .hero {
            margin-top: 80px;
            padding: 4rem 0;
            text-align: center;
            color: white;
        }

        .hero-content {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 3rem;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            animation: fadeInUp 1s ease;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            opacity: 0.9;
            animation: fadeInUp 1s ease 0.2s both;
        }

        .hero p {
            font-size: 1.1rem;
            margin-bottom: 2rem;
            opacity: 0.8;
            animation: fadeInUp 1s ease 0.4s both;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
            margin-bottom: 2rem;
            animation: fadeInUp 1s ease 0.6s both;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            background: rgba(255, 255, 255, 0.2);
            padding: 0.5rem 1rem;
            border-radius: 25px;
            transition: transform 0.3s ease;
        }

        .contact-item:hover {
            transform: translateY(-2px);
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(45deg, #ff6b6b, #ee5a6f);
            color: white;
            padding: 1rem 2rem;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(238, 90, 111, 0.4);
            animation: fadeInUp 1s ease 0.8s both;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(238, 90, 111, 0.6);
        }

        /* Sections */
        .section {
            padding: 4rem 0;
            background: white;
            margin: 2rem 0;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .section h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #333;
            position: relative;
        }

        .section h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(45deg, #667eea, #764ba2);
            border-radius: 2px;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .skill-category {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .skill-category:hover {
            transform: translateY(-5px);
        }

        .skill-category h3 {
            color: #667eea;
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .skill-tag {
            background: #667eea;
            color: white;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.9rem;
            transition: all 0.3s ease;
        }

        .skill-tag:hover {
            background: #764ba2;
            transform: scale(1.05);
        }

        /* Experience Timeline */
        .timeline {
            position: relative;
            max-width: 1000px;
            margin: 0 auto;
        }

        .timeline::after {
            content: '';
            position: absolute;
            width: 4px;
            background: linear-gradient(45deg, #667eea, #764ba2);
            top: 0;
            bottom: 0;
            left: 50%;
            margin-left: -2px;
        }

        .timeline-item {
            padding: 10px 40px;
            position: relative;
            background-color: inherit;
            width: 50%;
            margin-bottom: 2rem;
        }

        .timeline-item::after {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            right: -10px;
            background: #667eea;
            border: 4px solid white;
            top: 15px;
            border-radius: 50%;
            z-index: 1;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }

        .left {
            left: 0;
        }

        .right {
            left: 50%;
        }

        .right::after {
            left: -10px;
        }

        .timeline-content {
            padding: 2rem;
            background: white;
            position: relative;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .timeline-content:hover {
            transform: translateY(-5px);
        }

        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .project-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(255,255,255,0.1) 0%, rgba(255,255,255,0) 100%);
            pointer-events: none;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(102, 126, 234, 0.4);
        }

        .project-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .project-duration {
            background: rgba(255, 255, 255, 0.2);
            padding: 0.3rem 0.8rem;
            border-radius: 15px;
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin: 1rem 0;
        }

        .tech-item {
            background: rgba(255, 255, 255, 0.2);
            padding: 0.2rem 0.6rem;
            border-radius: 10px;
            font-size: 0.8rem;
        }

        /* Certifications */
        .cert-badge {
            display: inline-flex;
            align-items: center;
            background: linear-gradient(45deg, #4CAF50, #45a049);
            color: white;
            padding: 1rem 2rem;
            border-radius: 30px;
            font-weight: bold;
            box-shadow: 0 5px 15px rgba(76, 175, 80, 0.3);
            transition: transform 0.3s ease;
        }

        .cert-badge:hover {
            transform: translateY(-3px);
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .hero-subtitle {
                font-size: 1.2rem;
            }

            .contact-info {
                flex-direction: column;
                align-items: center;
            }

            .timeline::after {
                left: 31px;
            }

            .timeline-item {
                width: 100%;
                padding-left: 70px;
                padding-right: 25px;
            }

            .timeline-item::before {
                left: 60px;
                border: medium solid white;
                border-width: 10px 10px 10px 0;
                border-color: transparent white transparent transparent;
            }

            .left::after, .right::after {
                left: 21px;
            }

            .right {
                left: 0%;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <nav class="nav container">
            <div class="logo">Ranjani Portfolio</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#education">Education</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>Somana Siva Ranjani</h1>
                <div class="hero-subtitle">Quality Assurance Engineer & BI Developer</div>
                <p>8+ years of expertise in Application Development, QA/Testing, Production Support, ETL and Reporting</p>
                
                <div class="contact-info">
                    <div class="contact-item">
                        <span>📱</span>
                        <span>7890000099</span>
                    </div>
                    <div class="contact-item">
                        <span>✉️</span>
                        <span>somanaranjani@gmail.com</span>
                    </div>
                    <div class="contact-item">
                        <span>📍</span>
                        <span>London, UK</span>
                    </div>
                </div>

                <a href="#projects" class="cta-button">View My Work</a>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="section">
        <div class="container">
            <h2>Technical Expertise</h2>
            
            <div class="skills-grid">
                <div class="skill-category fade-in">
                    <h3>🗄️ Databases</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">SQL Server 2008/2012/2018</span>
                        <span class="skill-tag">Oracle 11g</span>
                        <span class="skill-tag">T-SQL</span>
                    </div>
                </div>

                <div class="skill-category fade-in">
                    <h3>🔄 ETL & Integration</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">SSIS</span>
                        <span class="skill-tag">SSRS</span>
                        <span class="skill-tag">Azure Data Factory</span>
                        <span class="skill-tag">Informatica</span>
                        <span class="skill-tag">Encompass</span>
                    </div>
                </div>

                <div class="skill-category fade-in">
                    <h3>🧪 Testing & QA</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Manual Testing</span>
                        <span class="skill-tag">Functional Testing</span>
                        <span class="skill-tag">UAT</span>
                        <span class="skill-tag">API Testing</span>
                        <span class="skill-tag">Regression Testing</span>
                    </div>
                </div>

                <div class="skill-category fade-in">
                    <h3>📊 BI & Visualization</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Sisense</span>
                        <span class="skill-tag">Tableau</span>
                        <span class="skill-tag">Power BI</span>
                        <span class="skill-tag">SSAS Cubes</span>
                    </div>
                </div>

                <div class="skill-category fade-in">
                    <h3>🛠️ Tools & Methodologies</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">JIRA</span>
                        <span class="skill-tag">Azure DevOps</span>
                        <span class="skill-tag">Agile/Scrum</span>
                        <span class="skill-tag">ActiveBatch</span>
                        <span class="skill-tag">Postman</span>
                    </div>
                </div>

                <div class="skill-category fade-in">
                    <h3>☁️ Cloud & Modern Tech</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Microsoft Azure</span>
                        <span class="skill-tag">Azure SQL</span>
                        <span class="skill-tag">Azure Blob Storage</span>
                        <span class="skill-tag">Cloud Migration</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="section">
        <div class="container">
            <h2>Professional Journey</h2>
            
            <div class="timeline">
                <div class="timeline-item left fade-in">
                    <div class="timeline-content">
                        <h3>Software Analyst</h3>
                        <h4>SEFE, London</h4>
                        <span class="project-duration">Jan 2022 - Present</span>
                        <p>Leading end-to-end QA operations for energy trading systems, specializing in ETL validation, regulatory compliance testing, and data integrity assurance across complex ETRM environments.</p>
                    </div>
                </div>

                <div class="timeline-item right fade-in">
                    <div class="timeline-content">
                        <h3>Senior Software Engineer</h3>
                        <h4>Accenture, India</h4>
                        <span class="project-duration">Nov 2020 - Sep 2021</span>
                        <p>Developed and maintained Azure Data Factory pipelines, implemented BI solutions, and provided production support for enterprise-level data integration projects.</p>
                    </div>
                </div>

                <div class="timeline-item left fade-in">
                    <div class="timeline-content">
                        <h3>Software Engineer</h3>
                        <h4>HCL, India</h4>
                        <span class="project-duration">Sep 2014 - Aug 2019</span>
                        <p>Built expertise in ETL development, database testing, and quality assurance across multiple projects, focusing on SSIS package development and comprehensive testing strategies.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="section">
        <div class="container">
            <h2>Key Projects</h2>
            
            <div class="projects-grid">
                <div class="project-card fade-in">
                    <h3>I&R Technical QA</h3>
                    <div class="project-duration">Jan 2022 - Present</div>
                    <p>Led comprehensive QA operations for energy trading data integration, ensuring seamless flow from ETRM systems to SAP while maintaining regulatory compliance.</p>
                    
                    <div class="tech-stack">
                        <span class="tech-item">SQL Server</span>
                        <span class="tech-item">Oracle</span>
                        <span class="tech-item">SSIS</span>
                        <span class="tech-item">SSRS</span>
                        <span class="tech-item">ENDUR</span>
                        <span class="tech-item">ADF</span>
                    </div>

                    <ul style="margin-top: 1rem; padding-left: 1rem;">
                        <li>Validated PnL positions and APAR transactions integration</li>
                        <li>Executed regression testing for EMIR and REMIT compliance</li>
                        <li>Designed reconciliation test scenarios using T-SQL</li>
                        <li>Managed defect tracking via Azure DevOps</li>
                    </ul>
                </div>

                <div class="project-card fade-in">
                    <h3>Custom Factory</h3>
                    <div class="project-duration">Jan 2018 - Sep 2021</div>
                    <p>Developed and maintained BI solutions with focus on Azure cloud migration, data pipeline optimization, and dashboard creation.</p>
                    
                    <div class="tech-stack">
                        <span class="tech-item">Azure Data Factory</span>
                        <span class="tech-item">Informatica</span>
                        <span class="tech-item">Sisense</span>
                        <span class="tech-item">Power BI</span>
                        <span class="tech-item">Azure SQL</span>
                    </div>

                    <ul style="margin-top: 1rem; padding-left: 1rem;">
                        <li>Migrated data from on-premises to Azure cloud</li>
                        <li>Built automated ADF pipelines with dependencies</li>
                        <li>Created interactive dashboards and reports</li>
                        <li>Optimized SQL queries for performance improvement</li>
                    </ul>
                </div>

                <div class="project-card fade-in">
                    <h3>Alberta Go Digital</h3>
                    <div class="project-duration">May 2015 - Dec 2017</div>
                    <p>Modernized legacy ETL processes by consolidating DTS packages into efficient SSIS solutions with comprehensive testing coverage.</p>
                    
                    <div class="tech-stack">
                        <span class="tech-item">SSIS 2008</span>
                        <span class="tech-item">SQL Server 2008 R2</span>
                        <span class="tech-item">VSTS</span>
                        <span class="tech-item">DTS Migration</span>
                    </div>

                    <ul style="margin-top: 1rem; padding-left: 1rem;">
                        <li>Consolidated 15 legacy DTS packages into single SSIS package</li>
                        <li>Performed comprehensive database testing and validation</li>
                        <li>Developed automated SQL Server job scheduling</li>
                        <li>Led QA standards implementation and testing automation</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Education & Certifications -->
    <section id="education" class="section">
        <div class="container">
            <h2>Education & Certifications</h2>
            
            <div style="text-align: center; margin-bottom: 3rem;">
                <div class="cert-badge fade-in">
                    🏆 Microsoft Azure Certified - Azure Fundamentals
                </div>
            </div>

            <div style="text-align: center;">
                <div class="timeline-content fade-in" style="display: inline-block; max-width: 600px;">
                    <h3>Bachelor's in Electronics and Communication Engineering</h3>
                    <h4>Osmania University</h4>
                    <span class="project-duration">Graduated 2014</span>
                    <p>Strong foundation in engineering principles with focus on electronics, communication systems, and technical problem-solving skills.</p>
                </div>
            </div>
        </div>
    </section>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Fade in animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Header background change on scroll
        window.addEventListener('scroll', () => {
            const header = document.querySelector('.header');
            if (window.scrollY > 100) {
                header.style.background = 'linear-gradient(135deg, #667eea 0%, #764ba2 100%)';
                header.style.opacity = '0.95';
            } else {
                header.style.background = 'linear-gradient(135deg, #667eea 0%, #764ba2 100%)';
                header.style.opacity = '1';
            }
        });

        // Add hover effects to project cards
        document.querySelectorAll('.project-card').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-10px) scale(1.02)';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(-10px) scale(1)';
            });
        });
    </script>
</body>
</html>
