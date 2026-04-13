[index (4).html](https://github.com/user-attachments/files/26663430/index.4.html)
# gsloan5579-rgb.github.io<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grant Sloan - Professional Portfolio</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary-blue: #2c3e50;
            --secondary-blue: #34495e;
            --light-gray: #ecf0f1;
            --accent-blue: #3498db;
            --primary-green: #1b5e20;
            --secondary-green: #2e7d32;
            --light-beige: #f5f1e8;
            --accent-gold: #d4af37;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #2c3e50;
            background-color: #f8f9fa;
        }

        /* Navigation */
        .navbar {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--secondary-blue) 100%);
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        .navbar-brand {
            font-weight: 700;
            font-size: 1.5rem;
            color: white !important;
        }

        .nav-link {
            color: rgba(255,255,255,0.8) !important;
            margin-left: 1rem;
            transition: color 0.3s;
            cursor: pointer;
        }

        .nav-link:hover {
            color: white !important;
        }

        .nav-link.active {
            color: var(--accent-blue) !important;
            border-bottom: 2px solid var(--accent-blue);
        }

        /* Page Sections */
        .page-section {
            display: none;
            animation: fadeIn 0.5s ease-in;
        }

        .page-section.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--secondary-blue) 100%);
            color: white;
            padding: 4rem 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.25rem;
            margin-bottom: 2rem;
            opacity: 0.95;
        }

        .hero .btn {
            margin: 0 0.5rem;
        }

        /* Content Sections */
        .section {
            padding: 3rem 0;
            border-bottom: 1px solid var(--light-gray);
        }

        .section h2 {
            font-size: 2rem;
            font-weight: 700;
            color: var(--primary-blue);
            margin-bottom: 2rem;
            padding-bottom: 1rem;
            border-bottom: 3px solid var(--accent-blue);
        }

        /* Resume Styles */
        .resume-section {
            margin-bottom: 2.5rem;
        }

        .resume-section h3 {
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--secondary-blue);
            margin-bottom: 1.5rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .resume-item {
            margin-bottom: 1.75rem;
            padding: 1.5rem;
            background: white;
            border-left: 4px solid var(--accent-blue);
            border-radius: 4px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }

        .resume-item h4 {
            font-size: 1.1rem;
            font-weight: 700;
            color: var(--primary-blue);
            margin-bottom: 0.25rem;
        }

        .resume-item .meta {
            font-size: 0.95rem;
            color: var(--accent-blue);
            margin-bottom: 0.75rem;
            font-weight: 600;
        }

        .resume-item .meta-secondary {
            font-size: 0.85rem;
            color: #7f8c8d;
        }

        .resume-item ul {
            margin-bottom: 0;
            padding-left: 1.5rem;
        }

        .resume-item li {
            margin-bottom: 0.5rem;
            color: #555;
            line-height: 1.6;
        }

        /* Skills */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
        }

        .skill-badge {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            border-top: 3px solid var(--accent-blue);
        }

        .skill-badge h5 {
            color: var(--primary-blue);
            font-weight: 700;
            margin-bottom: 0.75rem;
        }

        .skill-badge p {
            color: #666;
            font-size: 0.95rem;
            margin-bottom: 0;
        }

        /* Golf Page Styles */
        .golf-page {
            background-color: var(--light-beige);
        }

        .golf-page .section h2 {
            color: var(--primary-green);
            border-bottom-color: var(--accent-gold);
        }

        .golf-content-box {
            background: white;
            padding: 2.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            border-left: 5px solid var(--secondary-green);
            margin-bottom: 2rem;
        }

        .golf-content-box h3 {
            font-size: 1.5rem;
            color: var(--primary-green);
            margin-bottom: 1.5rem;
            font-weight: 700;
            border-bottom: 3px solid var(--accent-gold);
            padding-bottom: 0.75rem;
        }

        .golf-content-box p {
            font-size: 1.05rem;
            color: #333;
            margin-bottom: 1.5rem;
        }

        /* Golf Lists */
        .main-list {
            list-style-type: decimal;
            padding-left: 2rem;
            margin: 1.5rem 0;
        }

        .main-list li {
            margin-bottom: 1.5rem;
            font-weight: 600;
            color: var(--primary-green);
            font-family: 'Arial', sans-serif;
        }

        .nested-list {
            list-style-type: circle;
            padding-left: 2rem;
            margin-top: 0.75rem;
            margin-bottom: 0;
        }

        .nested-list li {
            margin-bottom: 0.5rem;
            font-weight: 400;
            color: #333;
            font-family: 'Georgia', serif;
        }

        /* Image Gallery */
        .image-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .image-gallery img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
            transition: transform 0.3s ease;
        }

        .image-gallery img:hover {
            transform: scale(1.02);
        }

        /* Video Container */
        .video-container {
            position: relative;
            width: 100%;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
            margin: 2rem 0;
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }

        /* Tableau Container */
        .tableau-container {
            width: 100%;
            margin: 2rem 0;
            padding: 1rem;
            background-color: #f9f9f9;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        .tableauPlaceholder {
            width: 100%;
        }

        /* Footer */
        footer {
            background: var(--primary-blue);
            color: white;
            padding: 2rem 0;
            margin-top: 3rem;
            text-align: center;
        }

        footer a {
            color: var(--accent-blue);
            text-decoration: none;
            margin: 0 0.75rem;
        }

        footer a:hover {
            text-decoration: underline;
        }

        /* Buttons */
        .btn-primary {
            background-color: var(--accent-blue);
            border-color: var(--accent-blue);
        }

        .btn-primary:hover {
            background-color: #2980b9;
            border-color: #2980b9;
        }

        .btn-outline-light:hover {
            background-color: var(--accent-blue);
            border-color: var(--accent-blue);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .section h2 {
                font-size: 1.5rem;
            }

            .image-gallery {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container-lg">
            <a class="navbar-brand" href="javascript:void(0)">Grant Sloan</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link active" onclick="showPage('professional', this)">Professional</a></li>
                    <li class="nav-item"><a class="nav-link" onclick="showPage('golf', this)">Golf</a></li>
                    <li class="nav-item"><a class="nav-link" onclick="showPage('app', this)">Score Tracker</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Professional Page -->
    <div id="professional" class="page-section active">
        <!-- Hero Section -->
        <section class="hero" id="home">
            <div class="container-lg">
                <h1>Grant Sloan</h1>
                <p>BYU Pre-Business Student</p>
                <a href="javascript:void(0)" onclick="scrollToSection('experience')" class="btn btn-primary">View My Work</a>
                <a href="javascript:void(0)" onclick="showPage('golf', null)" class="btn btn-outline-light">Explore My Interests</a>
            </div>
        </section>

        <!-- About Section -->
        <section class="section" id="about">
            <div class="container-lg">
                <h2>About</h2>
                <div class="row">
                    <div class="col-lg-8">
                        <p style="font-size: 1.1rem; color: #555; line-height: 1.8;">
                            I'm a finance-driven student at Brigham Young University with a passion for investment analysis, portfolio management, and financial markets. Currently interning at Nelson Group of Companies, I'm actively developing expertise in market analysis, risk assessment, and strategic investment decisions. My background combines technical financial knowledge with strong leadership skills developed through both professional experience and service roles.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Education Section -->
        <section class="section" id="education">
            <div class="container-lg">
                <h2>Education</h2>
                <div class="resume-item">
                    <h4>Bachelor of Science in Pre-Business</h4>
                    <div class="meta">Brigham Young University, Provo, UT</div>
                    <p><strong>GPA:</strong> 3.64/4.00</p>
                    <p><strong>Expected Graduation:</strong> April 2029</p>
                    <p><strong>Involvement:</strong></p>
                    <ul>
                        <li>Finance Society Member</li>
                        <li>Private Banking and Wealth Management Association Club Member</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Experience Section -->
        <section class="section" id="experience">
            <div class="container-lg">
                <h2>Experience</h2>
                
                <div class="resume-item">
                    <h4>Investment Intern</h4>
                    <div class="meta">Nelson Group of Companies, Heber City, UT</div>
                    <div class="meta-secondary">October 2025 – Present</div>
                    <ul>
                        <li>Managing a diversified investment portfolio focused on income generation, analyzing market trends and risk factors, executing strategic allocations, and monitoring performance to maximize returns while mitigating potential losses</li>
                        <li>Partnering closely with fellow portfolio managers in detailed investment discussions, analyzing market conditions, evaluating opportunities and risks, and contributing actionable insights to guide portfolio strategy</li>
                    </ul>
                </div>

                <div class="resume-item">
                    <h4>Stock Pitch Competition Finalist</h4>
                    <div class="meta">Brigham Capital Stock Pitch Competition, Provo, UT</div>
                    <div class="meta-secondary">February 2026</div>
                    <ul>
                        <li>Collaborated in a team-based stock pitch competition at Brigham Young University, analyzing Futu Holdings' business model, revenue streams, growth catalysts, and market opportunities to develop a Buy recommendation</li>
                        <li>Delivered a structured, team-based presentation, strengthening skills in financial analysis, collaboration, and public speaking, while effectively communicating key investment insights and strategic recommendations to judges</li>
                    </ul>
                </div>

                <div class="resume-item">
                    <h4>Photo Booth Attendant</h4>
                    <div class="meta">The Photo Booth Guy, Chino, CA</div>
                    <div class="meta-secondary">October 2022 – April 2023</div>
                    <ul>
                        <li>Coordinated client communications regarding pricing, service options, and event logistics for a variety of events, ensuring a seamless experience, resolving issues proactively, and maintaining strong customer satisfaction</li>
                        <li>Handled and maintained a photo booth at various events, actively assisting guests, troubleshooting and resolving technical issues in real time, providing guidance to attendees, and ensuring a smooth experience for all participants</li>
                    </ul>
                </div>

                <div class="resume-item">
                    <h4>Heavy Machinery Operator</h4>
                    <div class="meta">Picture Perfect Construction, Glendora, CA</div>
                    <div class="meta-secondary">June 2021 – September 2023</div>
                    <ul>
                        <li>Operated heavy machinery and transported equipment and construction materials between multiple job sites, ensuring timely delivery, proper handling of all materials, and smooth, efficient operations throughout each project</li>
                        <li>Executed closely with job site managers and warehouse teams to ensure accurate delivery of products and materials to job sites, streamlining workflow, supporting project efficiency, and ensuring smooth operations across all projects</li>
                    </ul>
                </div>

                <div class="resume-item">
                    <h4>Volunteer Representative</h4>
                    <div class="meta">The Church of Jesus Christ of Latter-day Saints, Fort Collins, CO</div>
                    <div class="meta-secondary">October 2023 – September 2025</div>
                    <ul>
                        <li>Served as an assistant to the president, overseeing the needs of over 200 individuals, coordinating logistics including housing, transportation, and financial planning, and ensuring smooth operations across all organizational activities</li>
                        <li>Delivered monthly training presentations to groups of 40–80 individuals, developing and enhancing communication, leadership, and public speaking skills, while providing actionable guidance and encouragement to participants</li>
                        <li>Built meaningful relationships with individuals in smaller cities and communities, supporting their personal and spiritual growth and guiding them to strengthen relationships and find inner peace</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Skills Section -->
        <section class="section" id="skills">
            <div class="container-lg">
                <h2>Skills & Interests</h2>
                <div class="skills-container">
                    <div class="skill-badge">
                        <h5>Financial Analysis</h5>
                        <p>Investment analysis, portfolio management, market research</p>
                    </div>
                    <div class="skill-badge">
                        <h5>Leadership</h5>
                        <p>Team coordination, public speaking, organizational management</p>
                    </div>
                    <div class="skill-badge">
                        <h5>Eagle Scout</h5>
                        <p>Boy Scouts of America - Orchestrated volunteer landscaping project</p>
                    </div>
                    <div class="skill-badge">
                        <h5>Golf</h5>
                        <p>Passionate competitor in tournaments across multiple states</p>
                    </div>
                    <div class="skill-badge">
                        <h5>Ice Hockey</h5>
                        <p>Peaks Adult Hockey B League - Teamwork and competitive development</p>
                    </div>
                    <div class="skill-badge">
                        <h5>Problem Solving</h5>
                        <p>Technical troubleshooting, strategic analysis, issue resolution</p>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Golf Page -->
    <div id="golf" class="page-section golf-page">
        <section class="hero" style="background: linear-gradient(135deg, var(--primary-green) 0%, var(--secondary-green) 100%);">
            <div class="container-lg">
                <h1>⛳ Grant's Golf Journey</h1>
                <p>Exploring passion, competition, and the beautiful game of golf</p>
            </div>
        </section>

        <section class="section">
            <div class="container-lg">
                <div class="golf-content-box">
                    <h3 id="overview">My Golf Story</h3>
                    <p>Golf has been a significant part of my life. What started as a recreational activity has evolved into a competitive pursuit where I travel across different states to compete in tournaments and enjoy casual rounds with friends and fellow golfers. The game teaches discipline, patience, and mental fortitude—qualities that extend far beyond the course.</p>
                    
                    <div class="image-gallery">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/66/Pebble_Beach_Golf_Links_-_11th_green.jpg/1280px-Pebble_Beach_Golf_Links_-_11th_green.jpg" alt="Pebble Beach Golf Links famous oceanside course">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fd/Pelican_Hill_Golf_Club_Ocean_North_17_green.jpg/1280px-Pelican_Hill_Golf_Club_Ocean_North_17_green.jpg" alt="Pelican Hill Golf Course Newport Beach ocean views">
                    </div>
                </div>

                <div class="golf-content-box">
                    <h3 id="golf-guide">Golf Basics & What I Love About It</h3>
                    
                    <p>Golf is a sport with depth and nuance. Here's what makes it special:</p>

                    <ol class="main-list">
                        <li>
                            <strong>The Technical Aspects</strong>
                            <ul class="nested-list">
                                <li>Swing mechanics and form</li>
                                <li>Short game precision (chipping and putting)</li>
                                <li>Understanding club selection and distances</li>
                                <li>Reading greens and understanding slope</li>
                            </ul>
                        </li>
                        <li>
                            <strong>Competition & Community</strong>
                            <ul class="nested-list">
                                <li>Tournament play across different courses</li>
                                <li>Networking with golfers from various backgrounds</li>
                                <li>Travel to golf destinations</li>
                                <li>Building lasting friendships on the course</li>
                            </ul>
                        </li>
                        <li>
                            <strong>Mental & Personal Development</strong>
                            <ul class="nested-list">
                                <li>Managing pressure and emotions during competition</li>
                                <li>Focus and concentration over 4-5 hour rounds</li>
                                <li>Resilience after difficult shots or rounds</li>
                                <li>Setting and achieving golf-related goals</li>
                            </ul>
                        </li>
                        <li>
                            <strong>Course Exploration</strong>
                            <ul class="nested-list">
                                <li>Discovering unique courses in different states</li>
                                <li>Understanding course architecture and design</li>
                                <li>Adapting to different conditions and layouts</li>
                                <li>Building a personal collection of favorite courses</li>
                            </ul>
                        </li>
                    </ol>
                </div>

                <div class="golf-content-box">
                    <h3 id="video">Golf Fundamentals Video</h3>
                    <p>Check out this great video about golf fundamentals and improving your game:</p>
                    
                    <div class="video-container">
                        <iframe width="100%" height="400" src="https://www.youtube.com/embed/s5DVTFCVr6M" title="Golf Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>

                    <p style="margin-top: 1.5rem; font-style: italic; color: #666;">This video provides valuable insights into golf techniques and practice methods to improve your game. Feel free to learn and apply these principles!</p>
                </div>

                <div class="golf-content-box">
                    <h3 id="stats">Golf Statistics & Analytics</h3>
                    <p>Explore this interactive visualization of golf statistics and insights from the PGA Tour:</p>

                    <div class="tableau-container">
                        <iframe src="https://public.tableau.com/views/GolfDashboard/GolfDash?:embed=y&:showVizHome=no&:display_count=y&:display_static_image=y" width="100%" height="600" style="border: none;"></iframe>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Golf App Page -->
    <div id="app" class="page-section">
        <section style="background: linear-gradient(135deg, var(--primary-green) 0%, var(--secondary-green) 100%); color: white; padding: 3rem 0; text-align: center;">
            <div class="container-lg">
                <h1>⛳ Golf Score Tracker</h1>
                <p>Track your rounds, improve your game</p>
            </div>
        </section>

        <section class="section">
            <div class="container-lg">
                <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; margin-bottom: 2rem;">
                    <div style="background: white; padding: 2rem; border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);">
                        <h2 style="color: #1b5e20; margin-bottom: 1.5rem; font-size: 1.5rem; border: none;">Log a Round</h2>
                        
                        <div style="margin-bottom: 1.5rem;">
                            <label style="display: block; margin-bottom: 0.5rem; color: #333; font-weight: 600;">Course Name</label>
                            <input type="text" id="courseName" placeholder="e.g., Pebble Beach Golf Links" style="width: 100%; padding: 0.75rem; border: 2px solid #e0e0e0; border-radius: 6px; font-size: 1rem;">
                        </div>

                        <div style="margin-bottom: 1.5rem;">
                            <label style="display: block; margin-bottom: 0.5rem; color: #333; font-weight: 600;">Score</label>
                            <input type="number" id="score" placeholder="Enter your score" min="1" style="width: 100%; padding: 0.75rem; border: 2px solid #e0e0e0; border-radius: 6px; font-size: 1rem;">
                        </div>

                        <div style="margin-bottom: 1.5rem;">
                            <label style="display: block; margin-bottom: 0.5rem; color: #333; font-weight: 600;">Par</label>
                            <input type="number" id="par" placeholder="Course par (e.g., 72)" min="1" style="width: 100%; padding: 0.75rem; border: 2px solid #e0e0e0; border-radius: 6px; font-size: 1rem;">
                        </div>

                        <div style="margin-bottom: 1.5rem;">
                            <label style="display: block; margin-bottom: 0.5rem; color: #333; font-weight: 600;">Date</label>
                            <input type="date" id="date" style="width: 100%; padding: 0.75rem; border: 2px solid #e0e0e0; border-radius: 6px; font-size: 1rem;">
                        </div>

                        <div style="margin-bottom: 1.5rem;">
                            <label style="display: block; margin-bottom: 0.5rem; color: #333; font-weight: 600;">Number of Holes</label>
                            <select id="holes" style="width: 100%; padding: 0.75rem; border: 2px solid #e0e0e0; border-radius: 6px; font-size: 1rem;">
                                <option value="9">9 Holes</option>
                                <option value="18" selected>18 Holes</option>
                            </select>
                        </div>

                        <div style="margin-bottom: 1.5rem;">
                            <label style="display: block; margin-bottom: 0.5rem; color: #333; font-weight: 600;">Weather Conditions</label>
                            <select id="weather" style="width: 100%; padding: 0.75rem; border: 2px solid #e0e0e0; border-radius: 6px; font-size: 1rem;">
                                <option value="">Select weather...</option>
                                <option value="sunny">Sunny</option>
                                <option value="cloudy">Cloudy</option>
                                <option value="rainy">Rainy</option>
                                <option value="windy">Windy</option>
                                <option value="mixed">Mixed</option>
                            </select>
                        </div>

                        <div style="display: flex; gap: 0.75rem; margin-bottom: 1.5rem;">
                            <button onclick="addRound()" style="flex: 1; padding: 0.75rem 1.5rem; background: #2e7d32; color: white; border: none; border-radius: 6px; font-size: 1rem; font-weight: 600; cursor: pointer;">Log Round</button>
                            <button onclick="resetForm()" style="flex: 1; padding: 0.75rem 1.5rem; background: #e0e0e0; color: #333; border: none; border-radius: 6px; font-size: 1rem; font-weight: 600; cursor: pointer;">Clear Form</button>
                        </div>
                    </div>

                    <div style="background: white; padding: 2rem; border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);">
                        <h2 style="color: #1b5e20; margin-bottom: 1.5rem; font-size: 1.5rem; border: none;">Your Statistics</h2>
                        
                        <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 1rem; margin-bottom: 2rem;">
                            <div style="background: #f5f1e8; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #2e7d32; text-align: center;">
                                <div style="color: #666; font-size: 0.9rem; margin-bottom: 0.5rem;">Total Rounds</div>
                                <div style="font-size: 2rem; font-weight: 700; color: #1b5e20;" id="totalRounds">0</div>
                            </div>
                            <div style="background: #f5f1e8; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #2e7d32; text-align: center;">
                                <div style="color: #666; font-size: 0.9rem; margin-bottom: 0.5rem;">Best Score</div>
                                <div style="font-size: 2rem; font-weight: 700; color: #1b5e20;" id="bestScore">--</div>
                            </div>
                            <div style="background: #f5f1e8; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #2e7d32; text-align: center;">
                                <div style="color: #666; font-size: 0.9rem; margin-bottom: 0.5rem;">Average Score</div>
                                <div style="font-size: 2rem; font-weight: 700; color: #1b5e20;" id="avgScore">--</div>
                            </div>
                            <div style="background: #f5f1e8; padding: 1.5rem; border-radius: 8px; border-left: 4px solid #2e7d32; text-align: center;">
                                <div style="color: #666; font-size: 0.9rem; margin-bottom: 0.5rem;">Worst Score</div>
                                <div style="font-size: 2rem; font-weight: 700; color: #1b5e20;" id="worstScore">--</div>
                            </div>
                        </div>

                        <h3 style="color: #1b5e20; margin-bottom: 1rem; font-size: 1.2rem;">Recent Rounds</h3>
                        <div id="roundsList"></div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container-lg">
            <p style="margin-bottom: 1rem;">Grant Sloan | (626) 650-1350 | gsloan24@byu.edu</p>
            <div>
                <a href="https://www.linkedin.com/in/grantksloan13" target="_blank">
                    <i class="fab fa-linkedin"></i> LinkedIn
                </a>
            </div>
            <p style="margin-top: 1rem; opacity: 0.8; font-size: 0.9rem;">© 2026 Grant Sloan. All rights reserved.</p>
        </div>
    </footer>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/js/bootstrap.bundle.min.js"></script>
    <script src="https://public.tableau.com/javascripts/api/tableau-2.min.js"></script>

    <script>
        // Page Navigation
        function showPage(pageName, element) {
            // Hide all pages
            document.querySelectorAll('.page-section').forEach(page => {
                page.classList.remove('active');
            });

            // Show selected page
            document.getElementById(pageName).classList.add('active');

            // Update nav links
            document.querySelectorAll('.nav-link').forEach(link => {
                link.classList.remove('active');
            });
            if (element) {
                element.classList.add('active');
            } else {
                document.querySelectorAll('.nav-link').forEach(link => {
                    if (link.textContent.trim() === 'Golf') {
                        link.classList.add('active');
                    }
                });
            }

            // Scroll to top
            window.scrollTo(0, 0);
        }

        function scrollToSection(sectionId) {
            const section = document.getElementById(sectionId);
            if (section) {
                section.scrollIntoView({ behavior: 'smooth' });
            }
        }

        // Golf App Functions
        let rounds = JSON.parse(localStorage.getItem('golfRounds')) || [];

        // Set today's date as default
        document.getElementById('date').valueAsDate = new Date();

        function addRound() {
            const courseName = document.getElementById('courseName').value;
            const score = parseInt(document.getElementById('score').value);
            const par = parseInt(document.getElementById('par').value);
            const date = document.getElementById('date').value;
            const holes = document.getElementById('holes').value;
            const weather = document.getElementById('weather').value;

            if (!courseName || !score || !par || !date) {
                alert('Please fill in all required fields');
                return;
            }

            const round = {
                id: Date.now(),
                course: courseName,
                score: score,
                par: par,
                date: date,
                holes: holes,
                weather: weather,
                scoreToPar: score - par
            };

            rounds.unshift(round);
            localStorage.setItem('golfRounds', JSON.stringify(rounds));
            
            resetForm();
            updateStats();
            displayRounds();
        }

        function deleteRound(id) {
            if (confirm('Are you sure you want to delete this round?')) {
                rounds = rounds.filter(r => r.id !== id);
                localStorage.setItem('golfRounds', JSON.stringify(rounds));
                updateStats();
                displayRounds();
            }
        }

        function resetForm() {
            document.getElementById('courseName').value = '';
            document.getElementById('score').value = '';
            document.getElementById('par').value = '';
            document.getElementById('weather').value = '';
            document.getElementById('date').valueAsDate = new Date();
            document.getElementById('courseName').focus();
        }

        function updateStats() {
            const totalRounds = rounds.length;
            document.getElementById('totalRounds').textContent = totalRounds;

            if (totalRounds === 0) {
                document.getElementById('bestScore').textContent = '--';
                document.getElementById('avgScore').textContent = '--';
                document.getElementById('worstScore').textContent = '--';
                return;
            }

            const scores = rounds.map(r => r.score);
            const bestScore = Math.min(...scores);
            const worstScore = Math.max(...scores);
            const avgScore = (scores.reduce((a, b) => a + b, 0) / totalRounds).toFixed(1);

            document.getElementById('bestScore').textContent = bestScore;
            document.getElementById('avgScore').textContent = avgScore;
            document.getElementById('worstScore').textContent = worstScore;
        }

        function displayRounds() {
            const roundsList = document.getElementById('roundsList');
            
            if (rounds.length === 0) {
                roundsList.innerHTML = '<div style="text-align: center; color: #999; padding: 2rem; font-style: italic;">No rounds logged yet. Start tracking your game!</div>';
                return;
            }

            roundsList.innerHTML = rounds.map(round => {
                const scoreColor = round.scoreToPar < 0 ? '#2e7d32' : round.scoreToPar === 0 ? '#d4af37' : '#dc3545';
                
                return `
                    <div style="background: #f5f1e8; padding: 1.5rem; border-radius: 8px; margin-bottom: 1rem; display: flex; justify-content: space-between; align-items: center; border-left: 4px solid #d4af37;">
                        <div>
                            <div style="font-weight: 700; color: #1b5e20; font-size: 1.1rem;">${round.course}</div>
                            <div style="color: #666; font-size: 0.9rem; margin-top: 0.25rem;">${new Date(round.date).toLocaleDateString()} • ${round.holes} holes • ${round.weather || 'N/A'}</div>
                        </div>
                        <div style="display: flex; align-items: center; gap: 1rem;">
                            <div style="font-size: 1.5rem; font-weight: 700; color: ${scoreColor};">
                                ${round.score} <span style="font-size: 0.7em;">(${round.scoreToPar < 0 ? '' : '+'}${round.scoreToPar})</span>
                            </div>
                            <button onclick="deleteRound(${round.id})" style="background: #dc3545; color: white; border: none; padding: 0.5rem 0.75rem; border-radius: 4px; cursor: pointer; font-size: 0.85rem;">Delete</button>
                        </div>
                    </div>
                `;
            }).join('');
        }

        // Initialize
        updateStats();
        displayRounds();
    </script>
</body>
</html>
