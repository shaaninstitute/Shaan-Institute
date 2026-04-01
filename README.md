# Shaan-Institute<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shaan Institute | Skill Development Academy</title>
    <style>
        :root {
            --primary-color: #8E24AA; /* Deep Purple */
            --secondary-color: #F3E5F5; /* Light Purple */
            --text-color: #333;
            --bg-color: #FAFAFA;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        /* Header Navigation */
        header {
            background-color: white;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo-section {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .logo-section img {
            height: 60px;
            width: auto;
            border-radius: 5px;
        }

        .institute-info h1 {
            color: var(--primary-color);
            font-size: 1.5rem;
            margin-bottom: 2px;
        }

        .institute-info p {
            font-size: 0.8rem;
            color: #666;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        nav a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 600;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--primary-color);
        }

        /* Sections */
        section {
            padding: 60px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            color: var(--primary-color);
            margin-bottom: 40px;
            font-size: 2.2rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background-color: var(--primary-color);
            margin: 10px auto 0;
        }

        /* About Section */
        #about {
            background-color: var(--secondary-color);
            border-radius: 10px;
            text-align: center;
            padding: 40px;
            margin-top: 40px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        #about p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto;
        }

        /* Courses Section */
        .courses-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .course-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .course-card:hover {
            transform: translateY(-5px);
        }

        .course-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .course-content {
            padding: 20px;
        }

        .course-title {
            color: var(--primary-color);
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .course-details {
            margin-bottom: 15px;
            font-size: 0.95rem;
        }

        .course-details ul {
            padding-left: 20px;
            margin-top: 10px;
            color: #555;
        }

        .course-meta {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 15px;
            padding-top: 15px;
            border-top: 1px solid #eee;
            font-weight: bold;
            color: #444;
        }

        /* Contact/Enrolment Section */
        #enrolment {
            background-color: var(--primary-color);
            color: white;
            border-radius: 10px;
            padding: 40px;
            margin-bottom: 40px;
        }

        #enrolment .section-title {
            color: white;
        }

        #enrolment .section-title::after {
            background-color: white;
        }

        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            text-align: center;
            margin-top: 30px;
        }

        .contact-item h3 {
            margin-bottom: 10px;
            font-size: 1.2rem;
        }

        .contact-item a {
            color: var(--secondary-color);
            text-decoration: none;
        }
        
        .contact-item a:hover {
            text-decoration: underline;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #222;
            color: white;
        }

        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 15px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo-section">
                <img src="logo.jpg" alt="Shaan Institute Logo" onerror="this.src='https://via.placeholder.com/80x80?text=Logo'">
                <div class="institute-info">
                    <h1>Shaan Institute</h1>
                    <p>Skill Development Academy | Est. 2008 | Regd No: MAH/943/08</p>
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#courses">Courses</a></li>
                    <li><a href="#enrolment">Enrolment</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="about">
        <h2 class="section-title">About Us</h2>
        <p>
            Shaan Institute is a trustable institute; we have been giving our services in training and empowering women since 2008. Many of our students are exploring their career paths by upgrading their skills at Shaan Institute. The institute is proudly registered by the government.
        </p>
    </section>

    <section id="courses">
        <h2 class="section-title">Our Courses</h2>
        <div class="courses-grid">
            
            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1556905055-8f358a7a47b2?auto=format&fit=crop&w=600&q=80" alt="Fashion Designing">
                <div class="course-content">
                    <h3 class="course-title">Fashion Designing</h3>
                    <div class="course-details">
                        Comprehensive diploma covering all aspects of modern fashion design.
                    </div>
                    <div class="course-meta">
                        <span>Duration: 2 Years (18mo course + 6mo internship)</span>
                    </div>
                    <div class="course-meta">
                        <span>Fees: ₹60,000 (Instalments available)</span>
                    </div>
                </div>
            </div>

            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1601202864619-a1b606f71b9c?auto=format&fit=crop&w=600&q=80" alt="Embroidery">
                <div class="course-content">
                    <h3 class="course-title">Embroidery</h3>
                    <div class="course-details">
                        Learn multiple styles of professional embroidery:
                        <ul>
                            <li>Hand embroidery & Aari work</li>
                            <li>Mirror work & Aabla work</li>
                            <li>Badla work & Zardozi work</li>
                            <li>Fancy work & Qureshi work</li>
                            <li>Ribbon work</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1605280209590-76082c3580dd?auto=format&fit=crop&w=600&q=80" alt="Tailoring">
                <div class="course-content">
                    <h3 class="course-title">Tailoring</h3>
                    <div class="course-details">
                        Master the basics of garment creation: Designing making, cloth measurement, stitching, and cutting.
                    </div>
                    <div class="course-meta">
                        <span>Duration: 6 Months</span>
                    </div>
                    <div class="course-meta">
                        <span>Fees: ₹5,000</span>
                    </div>
                </div>
            </div>

            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1588666308061-ce1ee015fc4b?auto=format&fit=crop&w=600&q=80" alt="Advance Tailoring">
                <div class="course-content">
                    <h3 class="course-title">Advance Tailoring</h3>
                    <div class="course-details">
                        Take your skills to the next level: Designing making, cloth measurement, stitching, cutting, and Pattern making (ladies' outfits).
                    </div>
                    <div class="course-meta">
                        <span>Duration: 8 Months</span>
                    </div>
                    <div class="course-meta">
                        <span>Fees: ₹5,000</span>
                    </div>
                </div>
            </div>

            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1563124508-e8a32b9b70bb?auto=format&fit=crop&w=600&q=80" alt="Mehendi">
                <div class="course-content">
                    <h3 class="course-title">Mehendi</h3>
                    <div class="course-details">
                        Become a professional mehendi artist. Learn all types of mehendi designs and organic mehendi (cone) making.
                    </div>
                </div>
            </div>

            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1460661419201-fd4cecdf8a8b?auto=format&fit=crop&w=600&q=80" alt="Painting">
                <div class="course-content">
                    <h3 class="course-title">Painting</h3>
                    <div class="course-details">
                        Includes: Fibre painting, pot painting, Glass painting, Sand painting, Nib painting, Emboss painting, copper painting, and Bed sheet design.
                    </div>
                    <div class="course-meta">
                        <span>Duration: 3 Months</span>
                    </div>
                    <div class="course-meta">
                        <span>Fees: ₹3,000</span>
                    </div>
                </div>
            </div>

            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1556910103-1c02745a872f?auto=format&fit=crop&w=600&q=80" alt="Cooking">
                <div class="course-content">
                    <h3 class="course-title">Cooking</h3>
                    <div class="course-details">
                        Learn 40 dishes! All dishes are practically made (using homemade masala) and demonstrated in front of students.
                    </div>
                    <div class="course-meta">
                        <span>Fees: ₹5,000</span>
                    </div>
                </div>
            </div>

            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?auto=format&fit=crop&w=600&q=80" alt="Beautician">
                <div class="course-content">
                    <h3 class="course-title">Beautician</h3>
                    <div class="course-details">
                        Comprehensive beauty training: Make up artist, Bridal package, hairstyle, and professional saree and sharara draping.
                    </div>
                </div>
            </div>

        </div>
    </section>

    <section id="enrolment">
        <h2 class="section-title">Enrolment & Contact</h2>
        <p style="text-align: center; font-size: 1.1rem; margin-bottom: 20px;">
            Ready to upgrade your skills? Send your name and desired course to our email to start your enrolment process.
        </p>
        
        <div class="contact-info">
            <div class="contact-item">
                <h3>Email Us</h3>
                <p><a href="mailto:instituteshaan@gmail.com">instituteshaan@gmail.com</a></p>
            </div>
            <div class="contact-item">
                <h3>Call Us</h3>
                <p><a href="tel:+919819228098">+91 9819228098</a></p>
            </div>
            <div class="contact-item">
                <h3>Location</h3>
                <p><a href="https://maps.app.goo.gl/8rTfqzbT3E3nL6uj8?g_st=atm" target="_blank" rel="noopener noreferrer">View on Maps</a></p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Shaan Institute. All Rights Reserved. Regd No: MAH/943/08.</p>
    </footer>

</body>
</html>
