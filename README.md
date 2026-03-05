<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muawiyya Kira Nura | Chemical Engineer & Mentor</title>
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', 'Segoe UI', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            padding: 30px 20px;
        }

        /* Custom font fallback */
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 30px;
            box-shadow: 0 30px 60px rgba(0,0,0,0.3);
            overflow: hidden;
            animation: slideUp 0.8s ease;
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(120deg, #1e3c72, #2a5298, #1e3c72);
            background-size: 200% 200%;
            animation: gradientShift 8s ease infinite;
            color: white;
            padding: 60px 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            animation: rotate 20s linear infinite;
        }

        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .hero-content {
            position: relative;
            z-index: 1;
        }

        .hero h1 {
            font-size: 4em;
            font-weight: 700;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            letter-spacing: 2px;
            animation: fadeInDown 1s ease;
        }

        .hero .subtitle {
            font-size: 1.5em;
            opacity: 0.95;
            margin-bottom: 20px;
            font-weight: 300;
            animation: fadeInUp 1s ease 0.2s both;
        }

        .hero .badge {
            display: inline-block;
            background: rgba(255,255,255,0.2);
            backdrop-filter: blur(5px);
            padding: 12px 30px;
            border-radius: 50px;
            font-size: 1.1em;
            border: 2px solid rgba(255,255,255,0.3);
            animation: fadeIn 1s ease 0.4s both;
        }

        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

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

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Main Content */
        .main-content {
            padding: 50px 40px;
        }

        /* Section Headers */
        .section-title {
            display: flex;
            align-items: center;
            margin-bottom: 30px;
            position: relative;
        }

        .section-title h2 {
            font-size: 2.2em;
            font-weight: 600;
            color: #1e3c72;
            margin-right: 15px;
            position: relative;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 60%;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            border-radius: 2px;
        }

        .section-title i {
            font-size: 2.2em;
            color: #667eea;
            background: linear-gradient(135deg, #667eea20, #764ba220);
            padding: 10px;
            border-radius: 50%;
        }

        /* About Section */
        .about-card {
            background: linear-gradient(135deg, #f8f9fa, #ffffff);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            margin-bottom: 40px;
            border-left: 5px solid #667eea;
            transition: transform 0.3s ease;
        }

        .about-card:hover {
            transform: translateX(10px);
        }

        .about-card p {
            font-size: 1.1em;
            color: #555;
            line-height: 1.8;
        }

        /* Grid Layout for Cards */
        .grid-2 {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
            margin-bottom: 40px;
        }

        .grid-3 {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
            margin-bottom: 40px;
        }

        /* Card Style */
        .card {
            background: white;
            border-radius: 20px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            border: 1px solid rgba(102, 126, 234, 0.1);
            position: relative;
            overflow: hidden;
        }

        .card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            transform: scaleX(0);
            transform-origin: left;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 20px 40px rgba(102, 126, 234, 0.2);
        }

        .card:hover::before {
            transform: scaleX(1);
        }

        .card .date {
            color: #667eea;
            font-size: 0.9em;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 10px;
        }

        .card h3 {
            color: #1e3c72;
            font-size: 1.4em;
            margin-bottom: 10px;
        }

        .card .subhead {
            color: #666;
            font-weight: 500;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .card .subhead i {
            color: #667eea;
        }

        .card p {
            color: #555;
            line-height: 1.7;
        }

        /* Awards Special Card */
        .award-card {
            background: linear-gradient(135deg, #fff9e6, #ffffff);
            border: 2px solid #ffd70030;
            text-align: center;
        }

        .award-card i {
            font-size: 3em;
            color: #ffd700;
            margin-bottom: 15px;
        }

        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .skill-category {
            background: white;
            border-radius: 20px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            transition: transform 0.3s ease;
        }

        .skill-category:hover {
            transform: translateY(-5px);
        }

        .skill-category h3 {
            color: #1e3c72;
            font-size: 1.3em;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid #667eea;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .skill-category ul {
            list-style: none;
        }

        .skill-category li {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
            color: #555;
            font-weight: 500;
        }

        .skill-category li i {
            color: #667eea;
            width: 20px;
        }

        .skill-tag {
            display: inline-block;
            background: linear-gradient(135deg, #667eea20, #764ba220);
            color: #1e3c72;
            padding: 8px 16px;
            border-radius: 50px;
            margin: 5px;
            font-size: 0.9em;
            font-weight: 500;
            transition: all 0.3s ease;
        }

        .skill-tag:hover {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            transform: scale(1.05);
        }

        /* Stats Section */
        .stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin: 50px 0 30px;
        }

        .stat-item {
            text-align: center;
            padding: 25px;
            background: linear-gradient(135deg, #667eea10, #764ba210);
            border-radius: 20px;
            transition: transform 0.3s ease;
        }

        .stat-item:hover {
            transform: scale(1.05);
        }

        .stat-number {
            font-size: 2.5em;
            font-weight: 700;
            color: #1e3c72;
            margin-bottom: 5px;
        }

        .stat-label {
            color: #666;
            font-size: 0.95em;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* Footer */
        footer {
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            color: white;
            padding: 40px;
            text-align: center;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 20px;
        }

        .social-links a {
            color: white;
            font-size: 1.5em;
            width: 50px;
            height: 50px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            background: white;
            color: #1e3c72;
            transform: translateY(-5px) rotate(360deg);
        }

        footer p {
            opacity: 0.9;
            font-size: 1em;
        }

        footer a {
            color: #ffd700;
            text-decoration: none;
            font-weight: 600;
        }

        /* Responsive Design */
        @media (max-width: 900px) {
            .grid-2, .grid-3, .skills-container, .stats {
                grid-template-columns: 1fr;
            }
            
            .hero h1 {
                font-size: 2.5em;
            }
            
            .main-content {
                padding: 30px 20px;
            }
        }

        /* Floating Animation */
        .floating {
            animation: floating 3s ease infinite;
        }

        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }

        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }

        ::-webkit-scrollbar-thumb {
            background: linear-gradient(135deg, #667eea, #764ba2);
            border-radius: 5px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: linear-gradient(135deg, #764ba2, #667eea);
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Hero Section -->
        <section class="hero">
            <div class="hero-content">
                <h1>Muawiyya Kira Nura</h1>
                <div class="subtitle">Chemical Engineer | Mentor | Innovator</div>
                <div class="badge">
                    <i class="fas fa-star" style="margin-right: 8px;"></i>
                    Best Graduating Student - Katsina Engineering 2024/25
                </div>
            </div>
        </section>

        <!-- Main Content -->
        <div class="main-content">
            <!-- About Section -->
            <div class="section-title">
                <h2>About Me</h2>
                <i class="fas fa-user-astronaut floating"></i>
            </div>
            <div class="about-card">
                <p>I am a passionate and dedicated Chemical Engineering graduate from Ahmadu Bello University, Zaria, with a strong commitment to mentoring, STEM education, and industrial innovation. Recognized as the <strong>Best Graduating Student of Katsina Engineering Students (2024/25)</strong>, I thrive on simplifying complex concepts and inspiring the next generation of engineers. My mission is to bridge the gap between academic excellence and practical industrial application.</p>
            </div>

            <!-- Stats Section -->
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number">7+</div>
                    <div class="stat-label">Years of Study</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">2</div>
                    <div class="stat-label">Major Awards</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">100+</div>
                    <div class="stat-label">Students Mentored</div>
                </div>
            </div>

            <!-- Education & Experience Grid -->
            <div class="section-title">
                <h2>Education & Experience</h2>
                <i class="fas fa-graduation-cap floating"></i>
            </div>
            
            <div class="grid-2">
                <!-- Education Card -->
                <div class="card">
                    <div class="date">2018 – 2025</div>
                    <h3>Ahmadu Bello University, Zaria</h3>
                    <div class="subhead">
                        <i class="fas fa-university"></i>
                        Bachelor of Engineering (Chemical Engineering)
                    </div>
                    <p>Graduated as the <strong>Best Graduating Student of Katsina Engineering Students</strong> (2024/25). Focused on industrial chemical processing and process optimization.</p>
                </div>

                <!-- Class Tutor - University -->
                <div class="card">
                    <div class="date">2018 – 2025 · Volunteer</div>
                    <h3>Class Tutor</h3>
                    <div class="subhead">
                        <i class="fas fa-chalkboard-teacher"></i>
                        Ahmadu Bello University, Zaria
                    </div>
                    <p>Mentored final-year students in laboratory work, project reporting, and exam preparation. Collaborated with high-performers to simplify complex topics for peers, improving overall academic performance.</p>
                </div>
            </div>

            <!-- GSSS Experience -->
            <div class="card" style="margin-bottom: 40px;">
                <div class="date">Organizer / Class Tutor</div>
                <h3>Government Science Secondary School (GSSS) Musawa</h3>
                <div class="subhead">
                    <i class="fas fa-school"></i>
                    JETS Club Organizing Secretary
                </div>
                <p>Served as Organizing Secretary of the Junior Engineers, Technicians and Scientists (JETS) Club. Organized quizzes, debates, and STEM tutorials. Led a student entrepreneurship initiative on Vaseline production to inspire innovation. Active member of QUIDDSO (Quiz, Debate, and Dramatic Society).</p>
            </div>

            <!-- Awards Section -->
            <div class="section-title">
                <h2>Honours & Awards</h2>
                <i class="fas fa-trophy floating"></i>
            </div>
            
            <div class="grid-2">
                <div class="card award-card">
                    <i class="fas fa-crown"></i>
                    <h3>Best Graduating Student</h3>
                    <div class="subhead">Katsina Engineering Students 2024/25</div>
                    <div class="date">December 2025</div>
                    <p>Ahmadu Bello University, Zaria, Nigeria – Recognized for outstanding academic excellence among all engineering students from Katsina State.</p>
                </div>

                <div class="card award-card">
                    <i class="fas fa-medal"></i>
                    <h3>Governmental Bursary Award</h3>
                    <div class="subhead">Excellence in Academics</div>
                    <div class="date">January 2026</div>
                    <p>Katsina State Government, Nigeria – Awarded for exceptional academic performance and dedication to engineering studies.</p>
                </div>
            </div>

            <!-- Skills Section -->
            <div class="section-title">
                <h2>Skills & Expertise</h2>
                <i class="fas fa-cogs floating"></i>
            </div>

            <div class="skills-container">
                <!-- Technical Skills -->
                <div class="skill-category">
                    <h3><i class="fas fa-flask"></i> Technical</h3>
                    <div>
                        <span class="skill-tag">⚗️ Industrial Chemical Processing</span>
                        <span class="skill-tag">🌱 Bio-based Feedstock</span>
                        <span class="skill-tag">📊 Process Flow & Unit Operations</span>
                        <span class="skill-tag">✅ Quality Control & Safety</span>
                        <span class="skill-tag">🏭 Industrial Waste Management</span>
                    </div>
                </div>

                <!-- Digital Skills -->
                <div class="skill-category">
                    <h3><i class="fas fa-laptop-code"></i> Digital</h3>
                    <div>
                        <span class="skill-tag">📊 Data Entry</span>
                        <span class="skill-tag">📝 Microsoft Word</span>
                        <span class="skill-tag">📈 Microsoft Excel</span>
                        <span class="skill-tag">📽️ Microsoft PowerPoint</span>
                    </div>
                </div>

                <!-- Soft Skills -->
                <div class="skill-category">
                    <h3><i class="fas fa-heart"></i> Soft Skills</h3>
                    <div>
                        <span class="skill-tag">⏰ Time Management</span>
                        <span class="skill-tag">🧠 Quick Learner</span>
                        <span class="skill-tag">💪 Self Confidence</span>
                        <span class="skill-tag">🤝 Teamwork & Leadership</span>
                        <span class="skill-tag">🔄 Adaptability</span>
                        <span class="skill-tag">📖 Ease in Understanding Concepts</span>
                    </div>
                </div>
            </div>

            <!-- Call to Action / Contact -->
            <div style="text-align: center; margin: 50px 0 20px;">
                <p style="font-size: 1.2em; color: #666;">Let's connect and create something amazing together!</p>
            </div>
        </div>

        <!-- Footer -->
        <footer>
            <div class="social-links">
                <a href="#"><i class="fab fa-linkedin-in"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-researchgate"></i></a>
            </div>
            <p>© 2026 Muawiyya Kira Nura. Crafted with <i class="fas fa-heart" style="color: #ff6b6b;"></i> for GitHub Pages</p>
            <p style="margin-top: 10px; font-size: 0.9em;">
                <i class="fas fa-envelope"></i> muawiyya.kira@example.com · 
                <i class="fas fa-map-marker-alt"></i> Zaria, Nigeria
            </p>
            <p style="margin-top: 20px; font-size: 0.8em; opacity: 0.7;">
                <i class="fas fa-code"></i> Built with HTML5, CSS3 & Font Awesome
            </p>
        </footer>
    </div>
</body>
</html>