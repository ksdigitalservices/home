<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KS Digital Services | Premium Digital Solutions</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <style>
        :root {
            --primary: #4361ee;
            --primary-dark: #3a0ca3;
            --secondary: #f72585;
            --accent: #4ade80;
            --light: #f8fafc;
            --dark: #0f172a;
            --gray: #64748b;
            --border: #e2e8f0;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f8fafc;
            color: #334155;
            line-height: 1.6;
        }
        
        .navbar {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            padding: 1rem 0;
        }
        
        .navbar-brand {
            font-weight: 700;
            font-size: 1.8rem;
            color: var(--primary);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .navbar-brand i {
            color: var(--secondary);
        }
        
        .nav-link {
            font-weight: 500;
            color: var(--dark);
            padding: 0.5rem 1rem;
            border-radius: 6px;
            transition: all 0.3s ease;
        }
        
        .nav-link:hover {
            background-color: rgba(67, 97, 238, 0.1);
            color: var(--primary);
        }
        
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
            color: white;
            padding: 5rem 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
            opacity: 0.9;
        }
        
        .btn-primary {
            background-color: var(--primary);
            border: none;
            padding: 0.8rem 2rem;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .btn-secondary {
            background-color: var(--secondary);
            border: none;
            padding: 0.8rem 2rem;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .btn-secondary:hover {
            background-color: #d11479;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .section-title h2 {
            font-size: 2.2rem;
            font-weight: 700;
            color: var(--dark);
            margin-bottom: 1rem;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--primary);
            border-radius: 2px;
        }
        
        .section-title p {
            color: var(--gray);
            max-width: 600px;
            margin: 0 auto;
        }
        
        .services-section {
            padding: 5rem 0;
            background-color: white;
        }
        
        .service-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
            height: 100%;
            border: 1px solid var(--border);
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .card-icon {
            height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
            color: white;
            font-size: 3rem;
        }
        
        .card-content {
            padding: 1.5rem;
        }
        
        .card-content h3 {
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 0.8rem;
            color: var(--dark);
        }
        
        .card-content p {
            color: var(--gray);
            margin-bottom: 1.5rem;
        }
        
        .card-actions {
            display: flex;
            gap: 0.8rem;
        }
        
        .card-btn {
            flex: 1;
            padding: 0.6rem 1rem;
            border-radius: 6px;
            font-weight: 500;
            text-align: center;
            text-decoration: none;
            transition: all 0.3s ease;
            font-size: 0.9rem;
        }
        
        .card-btn.primary {
            background-color: var(--primary);
            color: white;
        }
        
        .card-btn.primary:hover {
            background-color: var(--primary-dark);
        }
        
        .card-btn.secondary {
            background-color: var(--secondary);
            color: white;
        }
        
        .card-btn.secondary:hover {
            background-color: #d11479;
        }
        
        .testimonials-section {
            padding: 5rem 0;
            background-color: #f1f5f9;
        }
        
        .testimonial-card {
            background: white;
            border-radius: 12px;
            padding: 2rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            height: 100%;
            position: relative;
        }
        
        .testimonial-card::before {
            content: """;
            position: absolute;
            top: 10px;
            left: 20px;
            font-size: 4rem;
            color: rgba(67, 97, 238, 0.1);
            font-family: Georgia, serif;
        }
        
        .testimonial-text {
            font-style: italic;
            margin-bottom: 1.5rem;
            position: relative;
            z-index: 1;
        }
        
        .testimonial-author {
            font-weight: 600;
            color: var(--dark);
        }
        
        .site-footer {
            background-color: var(--dark);
            color: white;
            padding: 4rem 0 0;
        }
        
        .footer-logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: white;
            margin-bottom: 1.5rem;
            display: inline-block;
        }
        
        .footer-about {
            margin-bottom: 1.5rem;
            opacity: 0.8;
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
        }
        
        .social-link {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: rgba(255,255,255,0.1);
            color: white;
            transition: all 0.3s ease;
        }
        
        .social-link:hover {
            background-color: var(--primary);
            transform: translateY(-3px);
        }
        
        .footer-heading {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 1.5rem;
            color: white;
        }
        
        .footer-links {
            list-style: none;
            padding: 0;
        }
        
        .footer-links li {
            margin-bottom: 0.8rem;
        }
        
        .footer-links a {
            color: rgba(255,255,255,0.8);
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .footer-links a:hover {
            color: white;
            padding-left: 5px;
        }
        
        .copyright {
            text-align: center;
            padding: 2rem 0;
            margin-top: 3rem;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: rgba(255,255,255,0.7);
            font-size: 0.9rem;
        }
        
        .whatsapp-float {
            position: fixed;
            width: 60px;
            height: 60px;
            bottom: 30px;
            right: 30px;
            background-color: #25D366;
            color: white;
            border-radius: 50%;
            text-align: center;
            font-size: 1.8rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        
        .whatsapp-float:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 20px rgba(0,0,0,0.3);
        }
        
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .section-title h2 {
                font-size: 1.8rem;
            }
            
            .card-actions {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-light sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">
                <i class="bi bi-laptop"></i> KS DIGITAL SERVICES
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#services">Services</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#testimonials">Testimonials</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact">Contact</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="https://maps.app.goo.gl/AyuLvmf3TYjp9fH6A">Location</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    
    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Premium Digital Solutions</h1>
            <p>Your trusted partner for all digital documentation and certification needs. Fast, reliable, and professional services.</p>
            <div class="d-flex gap-3 justify-content-center flex-wrap">
                <a href="#services" class="btn btn-primary">Explore Services</a>
                <a href="https://wa.me/7893845696" target="_blank" class="btn btn-secondary">Contact Us</a>
            </div>
        </div>
    </section>
    
    <!-- Services Section -->
    <section id="services" class="services-section">
        <div class="container">
            <div class="section-title">
                <h2>Our Services</h2>
                <p>Professional solutions for all your documentation needs</p>
            </div>
            
            <div class="row g-4">
                <!-- Passport Application -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-passport"></i>
                        </div>
                        <div class="card-content">
                            <h3>Passport Application</h3>
                            <p>Fast and reliable passport application services with expert guidance.</p>
                            <div class="card-actions">
                                <a href="/passport" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20to%20Apply%20for%20passport" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Marriage Certificate -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-heart-fill"></i>
                        </div>
                        <div class="card-content">
                            <h3>Marriage Certificate</h3>
                            <p>Official marriage certificate services with quick processing.</p>
                            <div class="card-actions">
                                <a href="/marriage" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20a%20MARRIAGE%20CERTIFICATE" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Birth Certificate -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-person-vcard"></i>
                        </div>
                        <div class="card-content">
                            <h3>Birth Certificate</h3>
                            <p>Get your official birth certificate quickly and easily.</p>
                            <div class="card-actions">
                                <a href="/birth" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20a%20BIRTH%20CERTIFICATE" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>
               
                <!-- Food License -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-cup-straw"></i>
                        </div>
                        <div class="card-content">
                            <h3>Food License</h3>
                            <p>FSSAI food license registration for restaurants and food businesses.</p>
                            <div class="card-actions">
                                <a href="/foodLicense" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20a%20food%20license" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Trade License -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-briefcase"></i>
                        </div>
                        <div class="card-content">
                            <h3>Trade License</h3>
                            <p>Trade license registration for commercial establishments.</p>
                            <div class="card-actions">
                                <a href="/tradeLicense" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20a%20trade%20license" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Labour License -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-person-gear"></i>
                        </div>
                        <div class="card-content">
                            <h3>Labour License</h3>
                            <p>Labor license registration for businesses with employees.</p>
                            <div class="card-actions">
                                <a href="/labourLicense" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20a%20labour%20license" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- MSME Certificate -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-building"></i>
                        </div>
                        <div class="card-content">
                            <h3>UDYAM Certificate</h3>
                            <p>MSME/UDYAM registration for small and medium enterprises.</p>
                            <div class="card-actions">
                                <a href="/msme" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20a%20UDYAM/MSME%20CERTIFICATE" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Voter ID Card -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-person-check"></i>
                        </div>
                        <div class="card-content">
                            <h3>VOTER ID CARD</h3>
                            <p>Voter ID card application and updates with quick processing.</p>
                            <div class="card-actions">
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20to%20Apply%20for%20Voter%20ID" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- PAN Card -->
                <div class="col-md-6 col-lg-4">
                    <div class="service-card">
                        <div class="card-icon">
                            <i class="bi bi-credit-card"></i>
                        </div>
                        <div class="card-content">
                            <h3>PAN CARD</h3>
                            <p>PAN card application and correction services with fast delivery.</p>
                            <div class="card-actions">
                                <a href="/pancard" class="card-btn primary">Details</a>
                                <a href="https://wa.me/7893845696?text=Hi%20I%20want%20to%20Apply%20for%20PAN%20card" target="_blank" class="card-btn secondary">Apply</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Testimonials Section -->
    <section id="testimonials" class="testimonials-section">
        <div class="container">
            <div class="section-title">
                <h2>Client Testimonials</h2>
                <p>Hear from our satisfied customers</p>
            </div>
            
            <div class="row g-4">
                <div class="col-md-6 col-lg-4">
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Received my UDYAM Certificate instantly. KS Digital Services made the process so simple and quick!"</p>
                        <div class="testimonial-author">- Murthy</div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Got my Aadhar Address updated in just 3 days. Their service is efficient and reliable."</p>
                        <div class="testimonial-author">- Raju Yadav</div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Received my trade license within 24 hours. Amazing speed and professionalism!"</p>
                        <div class="testimonial-author">- Vishnu</div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Quick service and very helpful, got my PAN in just 1 day. Highly recommended!"</p>
                        <div class="testimonial-author">- Jyothi</div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Saved me a lot of time, excellent experience. Will use their services again for sure."</p>
                        <div class="testimonial-author">- Renuka</div>
                    </div>
                </div>
                
                <div class="col-md-6 col-lg-4">
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Highly recommend for anyone needing quick document services. Professional and reliable."</p>
                        <div class="testimonial-author">- Shiva</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer id="contact" class="site-footer">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 mb-4">
                    <div class="footer-logo">KS DIGITAL SERVICES</div>
                    <p class="footer-about">Your trusted partner for all digital documentation and certification needs. Fast, reliable, and professional services.</p>
                    <div class="social-links">
                        <a href="https://wa.me/7893845696" target="_blank" class="social-link">
                            <i class="bi bi-whatsapp"></i>
                        </a>
                        <a href="https://www.instagram.com/ksdigitalservice/" target="_blank" class="social-link">
                            <i class="bi bi-instagram"></i>
                        </a>
                        <a href="https://www.youtube.com/@ksdigitalservice" target="_blank" class="social-link">
                            <i class="bi bi-youtube"></i>
                        </a>
                        <a href="https://www.linkedin.com/in/ksdigitalservices/" target="_blank" class="social-link">
                            <i class="bi bi-linkedin"></i>
                        </a>
                    </div>
                </div>
                
                <div class="col-lg-2 col-md-6 mb-4">
                    <h3 class="footer-heading">Pages</h3>
                    <ul class="footer-links">
                        <li><a href="/Terms">Terms</a></li>
                        <li><a href="/privacy">Privacy</a></li>
                        <li><a href="/contact">Contact</a></li>
                        <li><a href="/cancellation">Cancellation</a></li>
                        <li><a href="/shipping">Shipping</a></li>
                    </ul>
                </div>
                
                <div class="col-lg-3 col-md-6 mb-4">
                    <h3 class="footer-heading">Services</h3>
                    <ul class="footer-links">
                        <li><a href="#services">Passport Application</a></li>
                        <li><a href="#services">Marriage Certificate</a></li>
                        <li><a href="#services">Birth Certificate</a></li>
                        <li><a href="#services">PAN Card</a></li>
                        <li><a href="#services">Voter ID</a></li>
                    </ul>
                </div>
                
                <div class="col-lg-3 col-md-6 mb-4">
                    <h3 class="footer-heading">Contact Us</h3>
                    <ul class="footer-links">
                        <li><a href="tel:7893845696"><i class="bi bi-telephone me-2"></i>+91 7893845696</a></li>
                        <li><a href="mailto:info@ksdigitalservices.com"><i class="bi bi-envelope me-2"></i>info@ksdigitalservices.com</a></li>
                        <li><a href="https://maps.app.goo.gl/AyuLvmf3TYjp9fH6A" target="_blank"><i class="bi bi-geo-alt me-2"></i>Hyderabad, Telangana</a></li>
                        <li><a href="#"><i class="bi bi-clock me-2"></i>Mon-Sat: 7:00 AM - 9:30 PM</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 KS Digital Services. All rights reserved.</p>
            </div>
        </div>
    </footer>
    
    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me/7893845696" target="_blank" class="whatsapp-float">
        <i class="bi bi-whatsapp"></i>
    </a>
    
    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
    
    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
