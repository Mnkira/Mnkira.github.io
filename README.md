# Mnkira.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muawiyya Kira Nura | About Me</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f4f7f9;
            color: #2c3e50;
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            overflow: hidden;
        }

        header {
            background: #1e3c72;
            color: white;
            padding: 40px 30px;
            text-align: center;
        }

        header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            letter-spacing: 1px;
        }

        header p {
            font-size: 1.2em;
            opacity: 0.9;
            font-style: italic;
        }

        .content {
            padding: 40px 30px;
        }

        .section {
            margin-bottom: 35px;
        }

        .section h2 {
            color: #1e3c72;
            border-bottom: 3px solid #1e3c72;
            padding-bottom: 8px;
            margin-bottom: 20px;
            font-size: 1.8em;
            display: inline-block;
        }

        .section h3 {
            color: #2c3e50;
            margin-bottom: 5px;
            font-size: 1.3em;
        }

        .section .subhead {
            font-weight: 600;
            color: #1e3c72;
            margin-bottom: 5px;
        }

        .section .date {
            color: #7f8c8d;
            font-size: 0.9em;
            margin-bottom: 10px;
        }

        .section p {
            margin-bottom: 15px;
        }

        .experience-item, .award-item {
            margin-bottom: 25px;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 10px;
        }

        .skill-category {
            flex: 1 1 250px;
            background: #ecf0f1;
            padding: 15px;
            border-radius: 8px;
        }

        .skill-category h3 {
            color: #1e3c72;
            margin-bottom: 10px;
            font-size: 1.2em;
            border-bottom: 2px solid #1e3c72;
            padding-bottom: 5px;
        }

        .skill-category ul {
            list-style-type: none;
            padding-left: 0;
        }

        .skill-category li {
            margin-bottom: 8px;
            padding-left: 20px;
            position: relative;
        }

        .skill-category li::before {
            content: "▹";
            color: #1e3c72;
            position: absolute;
            left: 0;
        }

        footer {
            background: #1e3c72;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 0.9em;
        }

        footer a {
            color: #f1c40f;
            text-decoration: none;
        }

        @media (max-width: 600px) {
            header h1 { font-size: 2em; }
            .content { padding: 20px; }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Muawiyya Kira Nura</h1>
            <p>Engineering Graduate | Mentor & Tutor | Aspiring Chemical Engineer</p>
        </header>

        <div class="content">
            <!-- About / Summary -->
            <div class="section">
                <h2>About Me</h2>
                <p>I am a dedicated engineering graduate from Ahmadu Bello University, passionate about mentoring, STEM education, and industrial chemical processing. With a strong background in tutoring and organizing educational activities, I strive to inspire innovation and simplify complex concepts for learners. Recognized as the best graduating student of Katsina Engineering Students, I am eager to apply my technical and soft skills in real-world engineering challenges.</p>
            </div>

            <!-- Education -->
            <div class="section">
                <h2>Education</h2>
                <div class="experience-item">
                    <h3>Ahmadu Bello University, Zaria, Nigeria</h3>
                    <div class="date">2018 – 2025</div>
                    <p><strong>Bachelor of Engineering (Chemical Engineering)</strong> – Graduated as Best Graduating Student of Katsina Engineering Students (2024/25).</p>
                </div>
            </div>

            <!-- Experience -->
            <div class="section">
                <h2>Experience</h2>

                <div class="experience-item">
                    <h3>Class Tutor</h3>
                    <div class="subhead">Ahmadu Bello University, Zaria, Nigeria</div>
                    <div class="date">2018 – 2025 (Volunteer)</div>
                    <p>Volunteered as a guide and mentor to final year students, providing orientation on laboratory work, project reporting, and exam preparation. Collaborated with high-performing students to simplify complex topics for peers with learning difficulties. Conducted tutorials to improve students' understanding and performance.</p>
                </div>

                <div class="experience-item">
                    <h3>Organizer / Class Tutor</h3>
                    <div class="subhead">Government Science Secondary School (GSSS) Musawa</div>
                    <div class="date">(Dates not specified)</div>
                    <p>Served as Organizing Secretary of the Junior Engineers, Technicians and Scientists (JETS) Club. Organized educational activities including quizzes, debates, and tutorials to strengthen STEM engagement. Led a student entrepreneurship initiative on Vaseline production to inspire innovation and business skills. Active member of the Quiz, Debate, and Dramatic Society (QUIDDSO).</p>
                </div>
            </div>

            <!-- Honours and Awards -->
            <div class="section">
                <h2>Honours & Awards</h2>

                <div class="award-item">
                    <h3>Best Graduating Student of Katsina Engineering Students</h3>
                    <div class="date">December 2025</div>
                    <p>Ahmadu Bello University, Zaria, Nigeria – Recognized for outstanding academic achievement among engineering students from Katsina State.</p>
                </div>

                <div class="award-item">
                    <h3>Governmental Bursary Award of Excellence</h3>
                    <div class="date">January 2026</div>
                    <p>Katsina State Government, Nigeria – Awarded for exceptional academic performance and dedication.</p>
                </div>
            </div>

            <!-- Skills -->
            <div class="section">
                <h2>Skills</h2>
                <div class="skills">
                    <div class="skill-category">
                        <h3>Technical Skills</h3>
                        <ul>
                            <li>Industrial chemical processing</li>
                            <li>Bio-based feedstock handling</li>
                            <li>Process flow and unit operations</li>
                            <li>Quality control and safety practices</li>
                            <li>Industrial waste and by-product awareness</li>
                        </ul>
                    </div>
                    <div class="skill-category">
                        <h3>Digital Skills</h3>
                        <ul>
                            <li>Data Entry</li>
                            <li>Microsoft Office (Word, Excel, PowerPoint)</li>
                        </ul>
                    </div>
                    <div class="skill-category">
                        <h3>Soft Skills</h3>
                        <ul>
                            <li>Time Management</li>
                            <li>Ease in understanding concepts</li>
                            <li>Self Confidence</li>
                            <li>Teamwork and leadership</li>
                            <li>Quick Learning and Adaptability</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <footer>
            <p>© 2026 Muawiyya Kira Nura. Built with GitHub Pages.</p>
            <p>Contact: <a href="mailto: mnkira38@gmail.com">mnkira38@gmail.com</a> </p>
        </footer>
    </div>
</body>
</html>
