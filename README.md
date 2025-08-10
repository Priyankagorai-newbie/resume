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
    /* Glow */
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
    /* Content container */
    .content {
        position: relative;
        z-index: 2;
        margin: 40px;
        text-align: center;
    }
    h1 {
        font-size: 3rem;
        color: #fff;
        letter-spacing: 2px;
        margin-bottom: 20px;
        text-shadow: 0 0 10px #5a86ff, 0 0px 20px #fff4;
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
    }
    .section {
        background: rgba(255,255,255,0.95);
        padding: 22px 28px;
        margin-bottom: 25px;
        border-radius: 16px;
        box-shadow: 0 7px 28px rgba(90,134,255,0.10);
        transition: box-shadow 0.3s, transform 0.3s;
        text-align: left;
    }
    .section:hover {
        box-shadow: 0 14px 36px 2px #feb47ba8;
        transform: translateY(-3px) scale(1.01);
    }
    ul {
        margin-left: 25px;
        font-size: 1rem;
        color: #404c70;
    }
    a {
        color: #5A86FF;
        text-decoration: none;
        font-weight: 700;
    }
    a:hover {
        color: #FEB47B;
        text-shadow: 0 0 8px #feb47b88;
    }
    table {
        width: 100%;
        border-collapse: collapse;
        font-size: 0.95rem;
        margin-top: 15px;
    }
    th, td {
        border: 1.5px solid #5a86ff44;
        padding: 10px 15px;
    }
    th {
        background: linear-gradient(90deg, #5A86FF 0, #FEB47B 100%);
        color: white;
    }
    tr:nth-child(even) { background-color: #f0f8ff; }
    strong { color: #5A86FF; }
</style>
</head>
<body>
    <div class="cursor-glow" id="cursorGlow"></div>

    <div class="content">
        <h1>Priyanka Gorai</h1>

        <div class="section contact">
            <h2>Contact</h2>
            <p><strong>Email:</strong> <a href="mailto:goraipriyanka27@gmail.com">goraipriyanka27@gmail.com</a></p>
            <p><strong>Mobile No.:</strong> +91 70479 07820</p>
            <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/priyanka-gorai-98694a253" target="_blank">linkedin.com/in/priyanka-gorai-98694a253</a></p>
            <p><strong>GitHub:</strong> <a href="https://github.com/Priyankagorai-newbie" target="_blank">Priyankagorai-newbie</a></p>
        </div>

        <div class="section profile">
            <h2>Profile</h2>
            <p>I am Priyanka Gorai, a dedicated and enthusiastic final-year B.Tech student in Electrical Engineering at Kalyani Government Engineering College...</p>
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
                <li><strong>Vocational Training – Eastern Railway...</strong></li>
                <li><strong>Vocational Training – Mejia Thermal Power Plant...</strong></li>
                <li><strong>Technical Member – Robotics Society...</strong></li>
            </ul>
        </div>

        <div class="section academics">
            <h2>Education</h2>
            <table>
                <tr><th>Qualification</th><th>Institution</th><th>Year</th><th>Percentage/Grade</th></tr>
                <tr><td>B.Tech</td><td>KGEC</td><td>2022-2026</td><td>-</td></tr>
                <tr><td>Class 12</td><td>DAV Public School</td><td>2022</td><td>First Division</td></tr>
                <tr><td>Class 10</td><td>DAV Public School</td><td>2020</td><td>90.80%</td></tr>
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
    if('ontouchstart' in window){
        glow.style.left = '50vw';
        glow.style.top = '40vh';
    }
    </script>
</body>
</html>
