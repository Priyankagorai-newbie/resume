<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Priyanka Gorai</title>
    <style>
        /* Animated Gradient Background */
        body {
            min-height: 100vh;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(120deg, #5A86FF, #7ED6DF, #FEB47B, #FF6E7F, #6DD5FA 90%);
            background-size: 400% 400%;
            animation: gradientFlow 12s ease infinite;
            color: #2e3a59;
        }
        @keyframes gradientFlow {
            0% {background-position: 0% 50%;}
            50% {background-position: 100% 50%;}
            100% {background-position: 0% 50%;}
        }
        /* Glowing Effect Overlay */
        .cursor-glow {
            position: fixed;
            top: 0; left: 0;
            width: 550px;
            height: 550px;
            pointer-events: none;
            z-index: 1;
            transform: translate(-50%, -50%);
            border-radius: 50%;
            background: radial-gradient(circle, rgba(255,255,255,0.25) 0%, rgba(255,255,255,0.03) 70%, transparent 100%);
            filter: blur(16px);
            opacity: 0.75;
            transition: background 0.35s;
        }
        /* Stacking content above glow */
        .content {
            position: relative;
            z-index: 2;
            margin: 40px;
        }
        h1 {
            text-align: center;
            font-size: 3rem;
            color: #20901c;
            letter-spacing: 2px;
            margin-bottom: 12px;
            text-shadow: 0 1px 10px #5a86ff, 0 0px 20px #fff4;
            animation: slideInX 0.7s 0.2s both;
        }
        h2 {
            color: #5A86FF;
            border-bottom: 3px solid #feb47b;
            padding-bottom: 7px;
            margin-bottom: 15px;
            font-weight: 700;
            font-size: 1.5rem;
            text-transform: uppercase;
            letter-spacing: 1.6px;
            text-shadow: 0 1px 5px #feb47b66;
            opacity: 0;
            animation: slideInX 0.7s forwards;
        }
        .section { 
            background: rgba(255,255,255,0.95);
            padding: 22px 28px;
            margin-bottom: 35px;
            border-radius: 16px;
            box-shadow: 0 7px 28px rgba(90,134,255,0.10);
            transition: box-shadow 0.3s, transform 0.3s;
            opacity: 0;
            animation: fadeIn 1s forwards;
        }
        .section:hover {
            box-shadow: 0 14px 36px 2px #feb47ba8;
            transform: translateY(-3px) scale(1.011);
        }
        .section:nth-of-type(1) { animation-delay: 0.4s; }
        .section:nth-of-type(2) { animation-delay: 0.6s; }
        .section:nth-of-type(3) { animation-delay: 0.8s; }
        .section:nth-of-type(4) { animation-delay: 1.0s; }
        .section:nth-of-type(5) { animation-delay: 1.2s; }
        .section:nth-of-type(6) { animation-delay: 1.4s; }
        @keyframes fadeIn { from {opacity:0;} to {opacity:1;} }
        @keyframes slideInX { from {opacity:0; transform:translateX(-40px);} to {opacity:1; transform:translateX(0);} }
        ul {
            margin-left: 25px;
            font-size: 1.05rem;
            color: #404c70;
        }
        a {
            color: #5A86FF;
            text-decoration: none;
            font-weight: 700;
            transition: color 0.2s, text-shadow 0.25s;
        }
        a:hover {
            color: #FEB47B;
            text-shadow: 0 0 9px #feb47b77;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.99rem;
            color: #2e3a59;
            margin-top: 15px;
        }
        th, td {
            border: 1.5px solid #5a86ff44;
            padding: 11px 16px;
            text-align: left;
        }
        th {
            background: linear-gradient(90deg, #5A86FF 0, #FEB47B 100%);
            color: #fff;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1.1px;
        }
        tr:nth-child(even) { background-color: #f0f8ff; }
        tr:hover { background: #ffe4e9; }
        strong { color: #5A86FF; }
        .contact p, .profile p {
            font-size: 1.09rem;
            color: #16325c;
        }
    </style>
</head>
<body>
    <div class="cursor-glow" id="cursorGlow"></div>
    <div class="content">
    <h1>Priyanka Gorai</h1>
    <p style="text-align: center; font-weight: 600; font-size: 1.22rem; color: #fff; text-shadow: 0 0 10px #5A86FF;">
        Electrical Engineering Student | B.Tech (4th Year)
    </p>
    <div class="section contact">
        <h2>Contact</h2>
        <p><strong>Email:</strong> <a href="mailto:goraipriyanka27@gmail.com">goraipriyanka27@gmail.com</a></p>
        <p><strong>Mobile No.:</strong> +91 70479 07820</p>
        <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/priyanka-gorai-98694a253" target="_blank" rel="noopener">linkedin.com/in/priyanka-gorai-98694a253</a></p>
        <p><strong>GitHub:</strong> <a href="https://github.com/Priyankagorai-newbie" target="_blank" rel="noopener">Priyankagorai-newbie</a></p>
    </div>
    <div class="section profile">
        <h2>Profile</h2>
        <p>I am Priyanka Gorai, a dedicated and enthusiastic final-year B.Tech student in Electrical Engineering at Kalyani Government Engineering College. Passionate about electrical systems, power generation, and automation, with strong analytical skills, teamwork abilities, and a commitment to continuous learning. Hands-on exposure through vocational training in industrial and power sectors.</p>
    </div>
    <div class="section skills">
        <h2>Skills</h2>
        <ul>
            <li>MS Office (Word, PowerPoint, Excel)</li>
            <li>MATLAB & Simulink</li>
            <li>Electrical Circuit Design & Testing</li>
            <li>Power Systems Fundamentals</li>
            <li>C Programming (Beginner), HTML (Beginner)</li>
            <li>Video Editing (Beginner)</li>
            <li>Creative & Technical Writing</li>
        </ul>
    </div>
    <div class="section experience">
        <h2>Work Experience & Training</h2>
        <ul>
            <li>
                <strong>Vocational Training – Eastern Railway, Asansol Division</strong> (June 2025 – July 2025)<br />
                Learned about electrical infrastructure and power distribution in Indian Railways.<br />
                Observed relay operations, control mechanisms, and high-voltage safety practices.
            </li>
            <li>
                <strong>Vocational Training – Mejia Thermal Power Plant (DVC), West Bengal</strong> (July 2024)<br />
                Gained exposure to thermal power generation processes, turbine operations, and SCADA systems.<br />
                Studied switchgear systems and power distribution methods.
            </li>
            <li>
                <strong>Technical Member – Robotics Society, KGEC</strong> (July 2023 – Present)<br />
                Worked as content coordinator for Smart Attendance System project.<br />
                Documented hardware logic, application flow, and proposals.
            </li>
            <li>
                <strong>Content Writing Intern – Conscript HR (Remote)</strong> (June 2025 – July 2025)<br />
                Wrote SEO-optimized articles and HR-related blogs.<br />
                Managed content for social media and promotional materials.
            </li>
            <li><strong>Volunteer – Team Everest NGO</strong> (June 2023 – July 2023)</li>
            <li><strong>Member – NSS (National Service Scheme), KGEC</strong> (2023 – Present)</li>
        </ul>
    </div>
    <div class="section academics">
        <h2>Education</h2>
        <table>
            <tr>
                <th>Qualification</th>
                <th>Institution</th>
                <th>Year</th>
                <th>Percentage/Grade</th>
            </tr>
            <tr>
                <td>B.Tech, Electrical Engineering (Ongoing)</td>
                <td>Kalyani Government Engineering College, WB (MAKAUT)</td>
                <td>2022 – 2026</td>
                <td>-</td>
            </tr>
            <tr>
                <td>Class 12 (Science)</td>
                <td>DAV Public School, CBSE</td>
                <td>2022</td>
                <td>First Division</td>
            </tr>
            <tr>
                <td>Class 10</td>
                <td>DAV Public School, CBSE</td>
                <td>2020</td>
                <td>90.80%</td>
            </tr>
        </table>
    </div>
    <div class="section hobbies">
        <h2>Hobbies</h2>
        <ul>
            <li>Writing stories and blogs</li>
            <li>Listening to songs</li>
            <li>Reading online articles</li>
            <li>Dancing</li>
        </ul>
    </div>
    </div>
    <script>
    // Cursor glow effect
    const glow = document.getElementById('cursorGlow');
    document.addEventListener('mousemove', (e) => {
        glow.style.left = e.clientX + 'px';
        glow.style.top = e.clientY + 'px';
    });
    // Touch devices fallback: glow to center
    if('ontouchstart' in window){
        glow.style.left = '50vw';
        glow.style.top = '40vh';
    }
    </script>
</body>
</html>
