# Shaan-Institute
Skill developmentacademy
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shaan Institute | Skill Development Academy (Est. 2008)</title>
    
    <!-- External Resources -->
    <link href="https://fonts.googleapis.com" rel="stylesheet">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css">

    <style>
        /* CSS STYLES */
        :root {
            --primary: #800020; /* Deep Burgundy */
            --accent: #D4AF37;  /* Indian Gold */
            --bg-light: #FFF9FA; /* Soft Silk Cream */
            --text-dark: #2d2d2d;
            --white: #ffffff;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* Navigation */
        header {
            background: var(--white);
            padding: 15px 5%;
            box-shadow: 0 2px 15px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 3px solid var(--accent);
        }

        nav { display: flex; justify-content: space-between; align-items: center; }
        .logo-box .name { font-family: 'Playfair Display', serif; font-size: 28px; color: var(--primary); font-weight: bold; letter-spacing: 1px; }
        .logo-box .est { font-size: 12px; color: var(--accent); font-weight: 600; text-transform: uppercase; margin-top: -5px; }

        nav ul { list-style: none; display: flex; gap: 25px; }
        nav ul li a { text-decoration: none; color: var(--text-dark); font-weight: 600; font-size: 14px; transition: 0.3s; }
        nav ul li a:hover { color: var(--primary); }

        /* Hero Section */
        .hero {
            height: 70vh;
            background: linear-gradient(rgba(128, 0, 32, 0.7), rgba(128, 0, 32, 0.7)), 
                        url('https://images.unsplash.com');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: var(--white);
            text-align: center;
            padding: 0 20px;
        }

        .hero h1 { font-family: 'Playfair Display', serif; font-size: 48px; margin-bottom: 10px; }
        .hero p { font-size: 18px; max-width: 600px; }

        /* Courses Grid */
        .container { width: 90%; max-width: 1200px; margin: auto; padding: 60px 0; }
        .section-title { text-align: center; font-family: 'Playfair Display', serif; color: var(--primary); font-size: 36px; margin-bottom: 40px; position: relative; }
        .section-title::after { content: ''; display: block; width: 60px; height: 3px; background: var(--accent); margin: 10px auto; }

        .course-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 25px; }
        .course-card { background: var(--white); border-radius: 12px; overflow: hidden; box-shadow: 0 5px 15px rgba(0,0,0,0.05); transition: 0.3s; border: 1px solid #eee; }
        .course-card:hover { transform: translateY(-10px); border-color: var(--accent); }
        .course-card img { width: 100%; height: 220px; object-fit: cover; }
        .course-card h3 { padding: 20px; text-align: center; color: var(--primary); font-family: 'Playfair Display', serif; }

        /* Actions Section (Enrollment/Verification) */
        .action-bg { background: #fdf2f4; padding: 80px 0; }
        .flex-box { display: flex; gap: 30px; flex-wrap: wrap; justify-content: center; }
        .card { background: var(--white); padding: 40px; border-radius: 15px; width: 350px; text-align: center; border-top: 6px solid var(--accent); box-shadow: 0 10px 30px rgba(0,0,0,0.05); }
        .card h3 { color: var(--primary); margin-bottom: 15px; }
        .card p { font-size: 14px; margin-bottom: 25px; color: #666; }
        .btn { display: inline-block; padding: 12px 30px; background: var(--primary); color: var(--white); text-decoration: none; border-radius: 5px; font-weight: 600; transition: 0.3s; }
        .btn:hover { background: #600018; transform: scale(1.05); }
        .btn.gold { background: var(--accent); color: #222; }

        /* Contact Footer */
        footer { background: #1a1a1a; color: #ccc; padding: 60px 0 20px; }
        .footer-content { text-align: center; }
        .footer-content a { color: var(--accent); text-decoration: none; }
        .footer-content p { margin: 10px 0; }
        .map-btn { display: inline-block; margin-top: 15px; padding: 8px 20px; border: 1px solid var(--accent); color: var(--accent); border-radius: 4px; text-decoration: none; font-size: 14px; transition: 0.3s; }
        .map-btn:hover { background: var(--accent); color: #000; }
        hr { border: 0; border-top: 1px solid #333; margin: 40px 0 20px; }

        /* Floating WhatsApp Button */
        .whatsapp-float {
            position: fixed;
            width: 60px; height: 60px;
            bottom: 30px; right: 30px;
            background-color: #25d366;
            color: #FFF;
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            transition: 0.3s;
        }
        .whatsapp-float:hover { transform: scale(1.1); color: #fff; }

        @media (max-width: 768px) {
            .hero h1 { font-size: 32px; }
            nav ul { display: none; } /* Mobile simplicity */
        }
    </style>
</head>
<body>

    <!-- Header Navigation -->
    <header>
        <nav class="container" style="padding:0">
            <div class="logo-box">
                <div class="name">SHAAN INSTITUTE</div>
                <div class="est">Established 2008</div>
            </div>
            <ul>
                <li><a href="#courses">Our Courses</a></li>
                <li><a href="#enroll">Enrollment</a></li>
                <li><a href="#verify">Verification</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Home Section -->
    <section class="hero">
        <h1>Master the Art of Fashion</h1>
        <p>Leading the way in professional skill development for women in Mumbra since 2008.</p>
    </section>

    <!-- Courses Section -->
    <section id="courses" class="container">
        <h2 class="section-title">Specialized Skill Courses</h2>
        <div class="course-grid">
            <div class="course-card">
                <img src="https://images.unsplash.com" alt="Fashion Designing">
                <h3>Fashion Designing</h3>
            </div>
            <div class="course-card">
                <img src="https://images.unsplash.com" alt="Embroidery">
                <h3>Hand Embroidery</h3>
            </div>
            <div class="course-card">
                <img src="https://images.unsplash.com" alt="Tailoring">
                <h3>Professional Tailoring</h3>
            </div>
            <div class="course-card">
                <img src="https://images.unsplash.com" alt="Mehendi">
                <h3>Bridal Mehendi Arts</h3>
            </div>
            <div class="course-card">
                <img src="https://images.unsplash.com" alt="Painting">
                <h3>Decorative Painting</h3>
            </div>
        </div>
    </section>

    <!-- Enrollment & Verification Section -->
    <section class="action-bg">
        <div class="container">
            <div class="flex-box">
                <!-- Enrollment -->
                <div id="enroll" class="card">
                    <h3>Course Enrollment</h3>
                    <p>Ready to start? Send your <b>Name</b> and <b>Course Choice</b> to our official email.</p>
                    <a href="mailto:instituteshaan@://gmail.com:" class="btn">Enroll via Email</a>
                </div>

                <!-- Verification -->
                <div id="verify" class="card">
                    <h3>Certificate Verification</h3>
                    <p>Employers can verify alumni by sending <b>Name</b>, <b>Course</b>, and <b>Completion Year</b>.</p>
                    <a href="mailto:instituteshaan@://gmail.com:" class="btn gold">Verify Certificate</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer / Contact Section -->
    <footer id="contact">
        <div class="container footer-content">
            <h2 style="color: var(--accent); font-family: 'Playfair Display', serif; margin-bottom: 20px;">Get In Touch</h2>
            <p>📞 <b>Phone:</b> <a href="tel:9819228098">9819228098</a></p>
            <p>📧 <b>Email:</b> <a href="mailto:instituteshaan@gmail.com">instituteshaan@gmail.com</a></p>
            <p>📍 <b>Location:</b> Behind Kausa Lake, Near Shimla Park, Mumbra, Thane.</p>
            <a href="https://maps.app.goo.gl" target="_blank" class="map-btn">Get Directions on Google Maps</a>
            
            <hr>
            <p style="font-size: 13px;">&copy; 2025 Shaan Institute. All Rights Reserved. Empowering skills since 2008.</p>
        </div>
    </footer>

    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me." class="whatsapp-float" target="_blank">
        <i class="fa fa-whatsapp"></i>
    </a>

</body>
</html>
