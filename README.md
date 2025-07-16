<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NEW HOME CONSTRUCTION & DESIGN | National City, CA</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            letter-spacing: -1px;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: #ffd700;
        }

        .contact-btn {
            background: linear-gradient(45deg, #ff6b35, #ff8c42);
            padding: 10px 25px;
            border-radius: 25px;
            text-decoration: none;
            color: white;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255,107,53,0.3);
        }

        .contact-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(255,107,53,0.4);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000"><polygon fill="rgba(255,255,255,0.1)" points="0,0 1000,300 1000,1000 0,700"/></svg>');
            background-size: cover;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            color: white;
            text-align: center;
            animation: slideInUp 1s ease-out;
        }

        @keyframes slideInUp {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 1rem;
            font-weight: 700;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .cta-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .cta-btn {
            display: inline-block;
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .cta-primary {
            background: linear-gradient(45deg, #ff6b35, #ff8c42);
            color: white;
            box-shadow: 0 8px 25px rgba(255,107,53,0.3);
        }

        .cta-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 35px rgba(255,107,53,0.4);
        }

        .cta-secondary {
            background: rgba(255,255,255,0.2);
            color: white;
            border: 2px solid rgba(255,255,255,0.3);
            backdrop-filter: blur(10px);
        }

        .cta-secondary:hover {
            background: rgba(255,255,255,0.3);
            transform: translateY(-3px);
        }

        /* Services Section */
        .services {
            padding: 100px 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }

        .section-title {
            text-align: center;
            font-size: 3rem;
            margin-bottom: 3rem;
            color: #333;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(45deg, #ff6b35, #ff8c42);
            border-radius: 2px;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background: white;
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(45deg, #ff6b35, #ff8c42);
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
            color: #ff6b35;
        }

        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: #333;
        }

        .service-card p {
            color: #666;
            line-height: 1.6;
        }

        /* About Section */
        .about {
            padding: 100px 0;
            background: white;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .about-text h2 {
            font-size: 2.5rem;
            margin-bottom: 2rem;
            color: #333;
        }

        .about-text p {
            font-size: 1.1rem;
            margin-bottom: 1.5rem;
            color: #666;
            line-height: 1.8;
        }

        .about-image {
            position: relative;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }

        .about-image::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, rgba(255,107,53,0.8), rgba(255,140,66,0.8));
            z-index: 1;
        }

        .about-image-placeholder {
            width: 100%;
            height: 400px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2rem;
            position: relative;
            z-index: 2;
        }

        /* Contact Section */
        .contact {
            padding: 100px 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }

        .contact-info h2 {
            font-size: 2.5rem;
            margin-bottom: 2rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 1.5rem;
        }

        .contact-icon {
            font-size: 1.5rem;
            margin-right: 1rem;
            color: #ffd700;
        }

        .contact-form {
            background: rgba(255,255,255,0.1);
            padding: 2rem;
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            color: white;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 10px;
            background: rgba(255,255,255,0.2);
            color: white;
            backdrop-filter: blur(5px);
        }

        .form-group input::placeholder,
        .form-group textarea::placeholder {
            color: rgba(255,255,255,0.7);
        }

        .submit-btn {
            background: linear-gradient(45deg, #ff6b35, #ff8c42);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
        }

        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(255,107,53,0.3);
        }

        /* Footer */
        footer {
            background: #1a1a1a;
            color: white;
            padding: 2rem 0;
            text-align: center;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: #ff6b35;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.2rem;
            }

            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }

            .about-content,
            .contact-content {
                grid-template-columns: 1fr;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">NH CONSTRUCTION</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <a href="#contact" class="contact-btn">Get Quote</a>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>NEW HOME CONSTRUCTION & DESIGN</h1>
                <p>Transform Your Vision Into Reality with Expert Construction Services in National City, CA</p>
                <div class="cta-buttons">
                    <a href="#contact" class="cta-btn cta-primary">Get Free Quote</a>
                    <a href="#services" class="cta-btn cta-secondary">Our Services</a>
                </div>
            </div>
        </div>
    </section>

    <section id="services" class="services">
        <div class="container">
            <h2 class="section-title">Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">🏠</div>
                    <h3>Custom Home Construction</h3>
                    <p>Build your dream home from the ground up with our expert custom home construction services. We handle everything from design to completion.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔨</div>
                    <h3>Home Remodeling</h3>
                    <p>Transform your existing space with our comprehensive home remodeling services. From concept to completion, we bring your vision to life.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">➕</div>
                    <h3>Home Additions</h3>
                    <p>Expand your living space with expertly designed and constructed home additions that seamlessly blend with your existing structure.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🍳</div>
                    <h3>Kitchen Remodeling</h3>
                    <p>Create the kitchen of your dreams with our minor to major kitchen remodeling services. Modern designs, quality materials, expert installation.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🪟</div>
                    <h3>Window Replacement</h3>
                    <p>Improve energy efficiency and curb appeal with our professional window replacement services. Quality windows, expert installation.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🌿</div>
                    <h3>Landscaping Improvements</h3>
                    <p>Enhance your outdoor living space with our landscaping improvement services. From design to installation, we create beautiful outdoor environments.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="about" class="about">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>About NEW HOME CONSTRUCTION & DESIGN</h2>
                    <p>Located in National City, CA, we are your trusted partner for all construction and remodeling needs. With years of experience in the industry, we specialize in new home construction, remodeling, and design services.</p>
                    <p>We serve the greater San Diego area including Bonita, Casa De Oro-Mount Helix, Coronado, Hill Crest San Diego, and Mission Hills San Diego. Our commitment to quality craftsmanship and customer satisfaction has made us a leading contractor in the region.</p>
                    <p>From custom homes to kitchen remodels, we handle projects of all sizes with the same dedication to excellence. Our experienced team works closely with you to ensure your vision becomes reality.</p>
                </div>
                <div class="about-image">
                    <div class="about-image-placeholder">
                        Professional Construction Team at Work
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <div class="contact-content">
                <div class="contact-info">
                    <h2>Get In Touch</h2>
                    <div class="contact-item">
                        <div class="contact-icon">📍</div>
                        <div>
                            <strong>Address:</strong><br>
                            2761 Ridgeway Dr<br>
                            National City, CA 91950
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">📞</div>
                        <div>
                            <strong>Phone:</strong><br>
                            (619) 372-4472
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">🌐</div>
                        <div>
                            <strong>Website:</strong><br>
                            nhcons.com
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">⏰</div>
                        <div>
                            <strong>Hours:</strong><br>
                            Mon-Fri: 8:00 AM - 6:00 PM<br>
                            Sat: 9:00 AM - 4:00 PM<br>
                            Sun: Closed
                        </div>
                    </div>
                </div>
                <div class="contact-form">
                    <h3>Request a Free Quote</h3>
                    <form>
                        <div class="form-group">
                            <label for="name">Name</label>
                            <input type="text" id="name" name="name" placeholder="Your Name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" name="email" placeholder="Your Email" required>
                        </div>
                        <div class="form-group">
                            <label for="phone">Phone</label>
                            <input type="tel" id="phone" name="phone" placeholder="Your Phone Number">
                        </div>
                        <div class="form-group">
                            <label for="service">Service Needed</label>
                            <select id="service" name="service" style="width: 100%; padding: 12px; border: none; border-radius: 10px; background: rgba(255,255,255,0.2); color: white; backdrop-filter: blur(5px);">
                                <option value="">Select a Service</option>
                                <option value="custom-home">Custom Home Construction</option>
                                <option value="remodeling">Home Remodeling</option>
                                <option value="additions">Home Additions</option>
                                <option value="kitchen">Kitchen Remodeling</option>
                                <option value="windows">Window Replacement</option>
                                <option value="landscaping">Landscaping Improvements</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="message">Message</label>
                            <textarea id="message" name="message" rows="4" placeholder="Tell us about your project..."></textarea>
                        </div>
                        <button type="submit" class="submit-btn">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="social-links">
                <a href="#" aria-label="Facebook">📘</a>
                <a href="#" aria-label="Instagram">📷</a>
            </div>
            <p>&copy; 2025 NEW HOME CONSTRUCTION & DESIGN. All rights reserved.</p>
            <p>Licensed Contractor | National City, CA | Serving San Diego County</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Form submission
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! We will contact you within 24 hours.');
            this.reset();
        });

        // Add scroll effect to header
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.background = 'rgba(30, 60, 114, 0.95)';
                header.style.backdropFilter = 'blur(10px)';
            } else {
                header.style.background = 'linear-gradient(135deg, #1e3c72 0%, #2a5298 100%)';
                header.style.backdropFilter = 'none';
            }
        });

        // Animate service cards on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.service-card').forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'translateY(30px)';
            card.style.transition = 'all 0.6s ease';
            observer.observe(card);
        });
    </script>
</body>
</html>
