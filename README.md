
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amazon Virtual Assistant | Professional Portfolio</title>
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background: linear-gradient(135deg, #232526 0%, #414345 100%);
            color: #f5f5f5;
            margin: 0;
            padding: 0;
            min-height: 100vh;
        }
        .container {
            max-width: 900px;
            margin: 48px auto;
            background: rgba(30, 30, 30, 0.93);
            border-radius: 22px;
            box-shadow: 0 8px 32px rgba(0,0,0,0.40);
            padding: 56px 42px 32px 42px;
            position: relative;
        }
        .profile-img {
            display: block;
            margin: 0 auto 22px auto;
            width: 180px;
            height: 180px;
            object-fit: cover;
            border-radius: 50%;
            border: 6px solid #fff;
            box-shadow: 0 4px 24px rgba(0,0,0,0.18);
            background: #eee;
            transition: box-shadow 0.2s;
        }
        .profile-img:hover {
            box-shadow: 0 8px 32px #0077b5;
        }
        .header {
            text-align: center;
            margin-bottom: 16px;
        }
        .header h1 {
            font-size: 2.9em;
            font-weight: 900;
            color: #fff;
            margin-bottom: 6px;
            letter-spacing: 2px;
        }
        .header h3 {
            font-size: 1.1em;
            color: #59d0ff;
            font-weight: 400;
            margin-top: 0;
            margin-bottom: 0;
        }
        .section {
            margin-top: 38px;
        }
        h2 {
            font-size: 1.4em;
            color: #59d0ff;
            margin-bottom: 12px;
            font-weight: 600;
            letter-spacing: 1px;
        }
        p, ul {
            font-size: 1.08em;
            line-height: 1.7;
            color: #e3e3e3;
        }
        ul {
            padding-left: 24px;
        }
        ul li {
            margin-bottom: 8px;
        }
        .services-list {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px 60px;
        }
        .experience, .testimonials {
            margin-top: 30px;
        }
        .testimonial {
            background: rgba(50, 50, 60, 0.7);
            border-radius: 14px;
            padding: 18px 22px;
            margin-bottom: 18px;
            border-left: 5px solid #59d0ff;
            font-style: italic;
        }
        .contact-btn {
            display: block;
            margin: 38px auto 0 auto;
            padding: 16px 42px;
            background-color: #59d0ff;
            color: #232526;
            font-size: 1.1em;
            font-weight: 700;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            box-shadow: 0 4px 18px rgba(89,208,255,0.16);
            transition: background 0.2s;
            text-decoration: none;
            text-align: center;
        }
        .contact-btn:hover {
            background-color: #41b4e6;
        }
        /* Hide contact info initially, reveal with fade-in */
        .contact-info-hidden {
            display: none;
            opacity: 0;
            transition: opacity 0.5s;
        }
        .contact-info-visible {
            display: block;
            opacity: 1;
            transition: opacity 0.5s;
        }
        @media (max-width: 660px) {
            .container {
                padding: 26px 10px 18px 10px;
            }
            .services-list {
                grid-template-columns: 1fr;
                gap: 10px 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Profile Image -->
        <img src="user-image-1.jpg" alt="Profile Picture" class="profile-img" />
        <div class="header">
            <h1>Amazon Virtual Assistant</h1>
            <h3>Professional Portfolio & Services</h3>
        </div>
        <div class="section about">
            <h2>About Me</h2>
            <p>
                Hi, I'm an experienced Amazon Virtual Assistant dedicated to helping sellers grow and manage their businesses on Amazon. With expertise in product research, listing optimization, PPC management, and account health maintenance, I provide end-to-end support tailored to your needs.
            </p>
        </div>
        <div class="section services">
            <h2>Services Offered</h2>
            <div class="services-list">
                <ul>
                    <li>Product Research & Sourcing</li>
                    <li>Listing Creation & Optimization</li>
                    <li>Inventory & Order Management</li>
                    <li>Amazon PPC Campaigns</li>
                </ul>
                <ul>
                    <li>Keyword Research</li>
                    <li>Account Health & Support</li>
                    <li>Competitor Analysis</li>
                    <li>Customer Service</li>
                </ul>
            </div>
        </div>
        <div class="section experience">
            <h2>Experience</h2>
            <p>
                Over 4 years supporting Amazon FBA & FBM sellers worldwide. Successfully launched and optimized dozens of products, managed ad budgets, and resolved account issues for various niches including Home, Beauty, and Electronics.
            </p>
        </div>
        <div class="section testimonials">
            <h2>Testimonials</h2>
            <div class="testimonial">
                "Fantastic VA! Helped grow my Amazon business with smart product choices and efficient listing optimization." <br> <strong>– Sarah J.</strong>
            </div>
            <div class="testimonial">
                "Highly recommend! My PPC performance improved dramatically and my account health is always in top shape." <br> <strong>– Michael B.</strong>
            </div>
        </div>
        <!-- Contact Section Start -->
        <div class="section contact">
            <h2>Contact Me</h2>
            <div id="contact-info" class="contact-info-hidden">
                <p>
                    📞 Phone: <a href="tel:+923099481292" style="color:#59d0ff;">+92 309 9481292</a><br>
                    📧 Email: <a href="mailto:info.amzvirtualassistant@gmail.com" style="color:#59d0ff;">info.amzvirtualassistant@gmail.com</a>
                </p>
            </div>
        </div>
        <button class="contact-btn" id="show-contact-btn">Contact Me</button>
        <!-- Contact Section End -->
    </div>
    <script>
        // Show contact info on button click
        document.getElementById('show-contact-btn').addEventListener('click', function() {
            var contactInfo = document.getElementById('contact-info');
            contactInfo.classList.remove('contact-info-hidden');
            contactInfo.classList.add('contact-info-visible');
            // Optionally disable the button after showing
            this.disabled = true;
            this.style.cursor = "default";
            this.textContent = "Contact Info Shown";
        });
    </script>
</body>
</html>
