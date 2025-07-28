<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Somana Siva Ranjani - Portfolio</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Abadi+MT:wght@400;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #d6eadf 0%, #e8f5e8 100%);
            color: #000;
            line-height: 1.6;
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            border-bottom: 2px solid rgba(0,0,0,0.1);
            margin-bottom: 40px;
        }

        .nav-menu {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .nav-menu li {
            font-weight: bold;
            font-size: 18px;
            cursor: pointer;
            transition: all 0.3s ease;
            padding: 10px 15px;
            border-radius: 25px;
        }

        .nav-menu li:hover {
            background: rgba(255,255,255,0.3);
            transform: translateY(-2px);
        }

        .name {
            font-size: 28px;
            font-weight: bold;
            color: #2c3e50;
        }

        .hero-section {
            display: grid;
            grid-template-columns: 250px 1fr;
            gap: 40px;
            margin-bottom: 50px;
            align-items: start;
        }

        .profile-card {
            background: rgba(255,255,255,0.9);
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            backdrop-filter: blur(10px);
        }

        .profile-placeholder {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 48px;
            font-weight: bold;
            border: 4px solid #fff;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .contact-info {
            margin-top: 20px;
            text-align: left;
        }

        .contact-info div {
            margin: 8px 0;
            font-size: 14px;
        }

        .about-section {
            background: rgba(255,255,255,0.9);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            backdrop-filter: blur(10px);
        }

        .about-section h2 {
            color: #2c3e50;
            margin-bottom: 20px;
            font-size: 24px;
            border-bottom: 3px solid #3498db;
            padding-bottom: 10px;
            display: inline-block;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin: 50px 0;
        }

        .skill-category {
            background: rgba(255,255,255,0.9);
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .skill-category:hover {
            transform: translateY(-5px);
        }

        .skill-category h3 {
            color: #2c3e50;
            margin-bottom: 15px;
            font-size: 18px;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-tag {
            background: linear-gradient(135deg, #3498db, #2980b9);
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
        }

        .experience-section {
            margin: 50px 0;
        }

        .section-title {
            font-size: 28px;
            color: #2c3e50;
            margin-bottom: 30px;
            text-align: center;
            font-weight: bold;
        }

        .experience-card {
            background: rgba(255,255,255,0.9);
            border-radius: 15px;
            padding: 30px;
            margin-bottom: 25px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            border-left: 5px solid #3498db;
        }

        .experience-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .job-title {
            font-size: 20px;
            font-weight: bold;
            color: #2c3e50;
        }

        .company {
            font-size: 16px;
            color: #7f8c8d;
        }

        .duration {
            background: #3498db;
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
        }

        .highlights {
            list-style: none;
            margin-top: 15px;
        }

        .highlights li {
            margin: 8px 0;
            padding-left: 20px;
            position: relative;
        }

        .highlights li:before {
            content: "▶";
            color: #3498db;
            position: absolute;
            left: 0;
        }

        .certifications {
            background: rgba(255,255,255,0.9);
            border-radius: 15px;
            padding: 25px;
            margin: 30px 0;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            text-align: center;
        }

        .cert-badge {
            display: inline-block;
            background: linear-gradient(135deg, #e74c3c, #c0392b);
            color: white;
            padding: 15px 25px;
            border-radius: 25px;
            font-weight: bold;
            margin: 10px;
            transform: rotate(-2deg);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        @media (max-width: 768px) {
            .hero-section {
                grid-template-columns: 1fr;
                text-align: center;
            }
            
            .nav-menu {
                flex-direction: column;
                gap: 10px;
            }
            
            header {
                flex-direction: column;
            }
            
            .experience-header {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <nav>
                <ul class="nav-menu">
                    <li onclick="scrollToSection('about')">ABOUT</li>
                    <li onclick="scrollToSection('skills')">SKILLS</li>
                    <li onclick="scrollToSection('experience')">EXPERIENCE</li>
                    <li onclick="scrollToSection('projects')">PROJECTS</li>
                </ul>
            </nav>
            <div class="name">SOMANA SIVA RANJANI</div>
        </header>

        <section class="hero-section" id="about">
            <div class="profile-card">
                
<img id="profileImage" src="" alt="Profile Photo" style="width: 180px; height: 180px; border-radius: 50%; object-fit: cover; border: 4px solid #fff; box-shadow: 0 5px 15px rgba(0,0,0,0.2); margin-bottom: 10px; background: #ddd;" />
<h3>Upload Profile Picture</h3>

<label style="display:block; margin-top: 10px; font-size: 14px;">From URL:</label>
<input type="url" id="profileUrlInput" placeholder="Paste image URL here" style="width: 100%; padding: 8px; border-radius: 8px; border: 1px solid #ccc;" />
<button onclick="updateProfileImage()" style="margin-top: 10px; padding: 8px 12px; background: #3498db; color: white; border: none; border-radius: 8px; cursor: pointer;">Use URL</button>

<label style="display:block; margin-top: 20px; font-size: 14px;">From Local File:</label>
<input type="file" id="profileFileInput" accept="image/*" style="margin-top: 5px;" onchange="loadLocalImage(event)" />

                
                <div class="contact-info">
                    <div><strong>📱</strong> 7890000099</div>
                    <div><strong>✉️</strong> somanaranjani@gmail.com</div>
                    <div><strong>📍</strong> London, UK</div>
                </div>
            </div>

            <div class="about-section">
                <h2>About Me</h2>
                <p>Seasoned QA/ETL professional with <strong>8+ years</strong> of expertise in application development, testing, and production support. Specialized in transforming complex business requirements into robust data solutions.</p>
                
                <p style="margin-top: 15px;">Expert in end-to-end ETL development using <strong>SSIS, Azure Data Factory</strong>, and cloud migration projects. Proven track record in <strong>manual testing, API validation</strong>, and <strong>Agile delivery</strong> for mission-critical applications.</p>
                
                <p style="margin-top: 15px;">Currently contributing as a <strong>Software Analyst at SEFE London</strong>, focusing on regulatory compliance, data integrity, and system optimization in energy trading environments.</p>
                
                <div class="certifications">
                    <div class="cert-badge">🏆 Microsoft Azure Certified</div>
                </div>
            </div>
        </section>

        <section id="skills">
            <h2 class="section-title">Technical Expertise</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>🗄️ Databases</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">SQL Server</span>
                        <span class="skill-tag">Oracle 11g</span>
                        <span class="skill-tag">T-SQL</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>🔄 ETL & Integration</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">SSIS</span>
                        <span class="skill-tag">Azure Data Factory</span>
                        <span class="skill-tag">Informatica</span>
                        <span class="skill-tag">SSRS</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>🧪 Testing & QA</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Manual Testing</span>
                        <span class="skill-tag">API Testing</span>
                        <span class="skill-tag">UAT</span>
                        <span class="skill-tag">Regression Testing</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>📊 Analytics & BI</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Sisense</span>
                        <span class="skill-tag">Tableau</span>
                        <span class="skill-tag">Power BI</span>
                        <span class="skill-tag">SSAS</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>🛠️ Tools & Platforms</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">JIRA</span>
                        <span class="skill-tag">Azure DevOps</span>
                        <span class="skill-tag">Postman</span>
                        <span class="skill-tag">ActiveBatch</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>⚡ Methodologies</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Agile/Scrum</span>
                        <span class="skill-tag">DevOps</span>
                        <span class="skill-tag">SDLC</span>
                        <span class="skill-tag">STLC</span>
                    </div>
                </div>
            </div>
        </section>

        <section id="experience">
            <h2 class="section-title">Professional Journey</h2>
            
            <div class="experience-card">
                <div class="experience-header">
                    <div>
                        <div class="job-title">Software Analyst</div>
                        <div class="company">SEFE, London</div>
                    </div>
                    <div class="duration">Jan 2022 - Present</div>
                </div>
                <ul class="highlights">
                    <li>Lead end-to-end QA for ETL solutions integrating energy trading systems (Endur) with SAP</li>
                    <li>Execute comprehensive testing across SSIS, SSRS, and regulatory reporting portals (EMIR/REMIT)</li>
                    <li>Validate complex financial data flows and reconciliation systems using T-SQL and SSRS</li>
                    <li>Collaborate with Agile teams to ensure production-ready solutions and maintain audit compliance</li>
                </ul>
            </div>

            <div class="experience-card">
                <div class="experience-header">
                    <div>
                        <div class="job-title">Senior Software Engineer</div>
                        <div class="company">Accenture, India</div>
                    </div>
                    <div class="duration">Nov 2020 - Sep 2021</div>
                </div>
                <ul class="highlights">
                    <li>Designed and maintained Azure Data Factory pipelines for cloud migration projects</li>
                    <li>Monitored production SSIS and Informatica jobs with proactive root cause analysis</li>
                    <li>Implemented BI dashboards using Sisense, Power BI, and Tableau for business insights</li>
                    <li>Optimized SQL queries and ETL processes to enhance system performance</li>
                </ul>
            </div>

            <div class="experience-card">
                <div class="experience-header">
                    <div>
                        <div class="job-title">Software Engineer</div>
                        <div class="company">HCL Technologies, India</div>
                    </div>
                    <div class="duration">Sep 2014 - Aug 2019</div>
                </div>
                <ul class="highlights">
                    <li>Developed and optimized SSIS packages, consolidating 15 legacy DTS packages into efficient solutions</li>
                    <li>Conducted comprehensive manual testing and created detailed test documentation</li>
                    <li>Automated package execution using SQL Server Agent with dependency management</li>
                    <li>Established QA standards and led quality assurance initiatives in Agile environments</li>
                </ul>
            </div>
        </section>

        <section id="projects">
            <h2 class="section-title">Key Projects</h2>
            
            <div class="experience-card">
                <div class="experience-header">
                    <div>
                        <div class="job-title">I&R Technical QA</div>
                        <div class="company">Energy Trading Data Integration</div>
                    </div>
                    <div class="duration">Current</div>
                </div>
                <ul class="highlights">
                    <li>Comprehensive testing of PnL positions and APAR transactions integration</li>
                    <li>Regulatory compliance validation for EMIR and REMIT reporting systems</li>
                    <li>API testing and deployment validation using Postman</li>
                </ul>
            </div>

            <div class="experience-card">
                <div class="experience-header">
                    <div>
                        <div class="job-title">Custom Factory</div>
                        <div class="company">Cloud Migration & BI Development</div>
                    </div>
                    <div class="duration">2018-2021</div>
                </div>
                <ul class="highlights">
                    <li>Azure Data Factory pipeline design for on-premises to cloud migration</li>
                    <li>Business intelligence dashboard development and maintenance</li>
                    <li>Production support with SLA-driven incident resolution</li>
                </ul>
            </div>

            <div class="experience-card">
                <div class="experience-header">
                    <div>
                        <div class="job-title">Alberta Go Digital</div>
                        <div class="company">Government Digital Transformation</div>
                    </div>
                    <div class="duration">2015-2017</div>
                </div>
                <ul class="highlights">
                    <li>ETL package development and comprehensive testing framework</li>
                    <li>Legacy system modernization and process optimization</li>
                    <li>Quality assurance leadership and Agile methodology implementation</li>
                </ul>
            </div>
        </section>
    </div>

    <script>
        function scrollToSection(sectionId) {
            document.getElementById(sectionId).scrollIntoView({
                behavior: 'smooth'
            });
        }

        // Add click functionality to profile photo placeholder
        document.querySelector('.profile-placeholder').addEventListener('click', function() {
            alert('Photo upload functionality can be implemented here');
        });

        // Add hover effects to skill tags
        document.querySelectorAll('.skill-tag').forEach(tag => {
            tag.addEventListener('mouseenter', function() {
                this.style.transform = 'scale(1.1)';
                this.style.transition = 'transform 0.2s ease';
            });
            
            tag.addEventListener('mouseleave', function() {
                this.style.transform = 'scale(1)';
            });
        });
    
function updateProfileImage() {
    const url = document.getElementById('profileUrlInput').value;
    const img = document.getElementById('profileImage');
    if (url) {
        img.src = url;
    } else {
        alert('Please enter a valid image URL.');
    }
}

function loadLocalImage(event) {
    const file = event.target.files[0];
    const img = document.getElementById('profileImage');
    
    if (file && file.type.startsWith('image/')) {
        const reader = new FileReader();
        reader.onload = function(e) {
            img.src = e.target.result;
        }
        reader.readAsDataURL(file);
    } else {
        alert('Please select a valid image file.');
    }
}

</script>
</body>
</html>
