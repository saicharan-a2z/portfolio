<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body, html {
            font-family: 'Roboto', sans-serif;
            height: 100%;
            background-color: #111;
            color: #fff;
            overflow-x: hidden;
        }

        /* Header */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            padding: 20px;
            z-index: 100;
            animation: slideDown 1s forwards;
        }

        header h1 {
            font-size: 2.5rem;
            color: #FFD700;
            letter-spacing: 2px;
            text-align: center;
        }

        @keyframes slideDown {
            0% { transform: translateY(-100%); }
            100% { transform: translateY(0); }
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
        }

        nav a {
            color: #fff;
            font-size: 1.2rem;
            text-decoration: none;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #FFD700;
        }

        /* Parallax Background */
        .parallax {
            position: relative;
            background: url('https://images.unsplash.com/photo-1517515019789-b3b2b6b8b6a0') no-repeat center center fixed;
            background-size: cover;
            height: 100vh;
            color: #fff;
            text-align: center;
        }

        .parallax h2 {
            font-size: 3rem;
            margin-top: 20%;
            letter-spacing: 5px;
        }

        /* Profile Section */
        #profile {
            text-align: center;
            padding: 100px 50px;
            animation: fadeIn 2s forwards;
            margin-top: 50px;
        }

        #profile img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 5px solid #FFD700;
            animation: scaleUp 2s ease-in-out forwards;
        }

        @keyframes scaleUp {
            0% { transform: scale(0); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }

        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }

        h2 {
            font-size: 2.5rem;
            margin-top: 20px;
        }

        p {
            font-size: 1.2rem;
            margin-top: 20px;
            line-height: 1.6;
        }

        /* Skills Section */
        #skills {
            padding: 80px 50px;
            text-align: center;
            animation: fadeInSection 2s forwards;
        }

        @keyframes fadeInSection {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }

        #skills h2 {
            font-size: 2.5rem;
        }

        .skills-container {
            display: flex;
            justify-content: center;
            gap: 40px;
            margin-top: 40px;
        }

        .skills-container i {
            font-size: 3.5rem;
            color: #FFD700;
            transition: transform 0.3s ease;
            cursor: pointer;
        }

        .skills-container i:hover {
            transform: scale(1.3);
        }

        /* Projects Section */
        #projects {
            padding: 100px 50px;
            background-color: #222;
            text-align: center;
            animation: fadeInSection 2s forwards;
        }

        #projects h2 {
            font-size: 2.5rem;
        }

        .project-card {
            display: inline-block;
            width: 250px;
            margin: 20px;
            background-color: #333;
            border-radius: 8px;
            overflow: hidden;
            position: relative;
            transition: transform 0.3s ease;
        }

        .project-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .project-card:hover {
            transform: translateY(-10px);
        }

        .project-card h3 {
            padding: 20px;
            background-color: #111;
            color: #fff;
            font-size: 1.5rem;
        }

        /* Contact Section */
        #contact {
            padding: 100px 50px;
            text-align: center;
            animation: fadeInSection 2s forwards;
        }

        #contact h2 {
            font-size: 2.5rem;
            margin-bottom: 30px;
        }

        .contact-form input, .contact-form textarea {
            width: 80%;
            padding: 15px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
            background-color: #222;
            color: #fff;
            font-size: 1.2rem;
        }

        .contact-form button {
            width: 80%;
            padding: 15px;
            background-color: #FFD700;
            border: none;
            border-radius: 5px;
            font-size: 1.2rem;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .contact-form button:hover {
            background-color: #e6b800;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 30px;
            background-color: #111;
            color: #fff;
        }

    </style>
</head>
<body>

    <!-- Parallax Background -->
    <div class="parallax">
        <header>
            <h1>SaiCharan Gollapalli</h1>
            <nav>
                <a href="#profile">Profile</a>
                <a href="#skills">Skills</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </nav>
        </header>
        <h2>Web Developer & Designer</h2>
    </div>

    <!-- Profile Section -->
    <section id="profile">
        <img src="https://media-maa2-1.cdn.whatsapp.net/v/t61.24694-24/465249692_1192989508448067_7688219996576908148_n.jpg?ccb=11-4&oh=01_Q5AaIJ8zV2eoEyKlEr5tzH12YnCP3cwfmmnbEB4rV37J5ZbZ&oe=67AA1F6E&_nc_sid=5e03e0&_nc_cat=107" alt="John Doe">
        <h2>About Me</h2>
        <p>I am a passionate web developer with expertise in front-end and back-end technologies. I specialize in building user-friendly, high-performance websites and applications.</p>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <h2>My Skills</h2>
        <div class="skills-container">
            <i class="fab fa-html5" title="HTML5"></i>
            <i class="fab fa-css3-alt" title="CSS3"></i>
            <i class="fab fa-js" title="JavaScript"></i>
            <i class="fab fa-react" title="React"></i>
            <i class="fab fa-node" title="Node.js"></i>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>My Projects</h2>
        <div class="project-card">
            <img src="https://tse4.mm.bing.net/th?id=OIP.yzH0Ap5FDo3snzq_nc9-fQHaFj&pid=Api&P=0&h=180" alt="Project 1">
            <h3>Project One</h3>
        </div>
        <div class="project-card">
            <img src="https://tse1.mm.bing.net/th?id=OIP.7nNyzIM61d0vjvbZnBC04gHaFj&pid=Api&P=0&h=180" alt="Project 2">
            <h3>Project Two</h3>
        </div>
        <div class="project-card">
            <img src="https://res.cloudinary.com/practicaldev/image/fetch/s--2dBpcyyl--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/rd575jvknxdiphinwmuj.jpg" alt="Project 3">
            <h3>Project Three</h3>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Me</h2>
        <form class="contact-form">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea rows="5" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 John Doe</p>
    </footer>

    <!-- External JS (FontAwesome icons) -->
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>

    <!-- Scroll-triggered Animation -->
    <script>
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                const sectionTop = section.getBoundingClientRect().top;
                if (sectionTop < window.innerHeight - 100) {
                    section.style.opacity = 1;
                }
            });
        });
    </script>

</body>
</html>
