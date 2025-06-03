<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Central Florida Property Services - Premier property management, cleaning, and marketing for vacation rentals in Orlando, Kissimmee, and Central Florida.">
    <meta name="keywords" content="property management Orlando, vacation rental cleaning Kissimmee, Central Florida property services, Airbnb management">
    <meta name="author" content="Central Florida Property Services">
    <title>Central Florida Property Services</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="icon" type="image/png" href="favicon.png"> <!-- Placeholder favicon -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <div class="logo">
                <!-- Replace with <img src="logo.png" alt="Your Logo" class="logo-img"> if you have a logo -->
                Central Florida Property Services
            </div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Us</a></li>
                <li class="dropdown">
                    <a href="#services" class="dropbtn">Property Management</a>
                    <div class="dropdown-content">
                        <a href="#services">Guest Support</a>
                        <a href="#services">Maintenance</a>
                        <a href="#services">Booking Management</a>
                    </div>
                </li>
                <li class="dropdown">
                    <a href="#services" class="dropbtn">Full-Service Cleanings</a>
                    <div class="dropdown-content">
                        <a href="#services">Deep Cleaning</a>
                        <a href="#services">Turnover Services</a>
                        <a href="#services">Eco-Friendly Options</a>
                    </div>
                </li>
                <li class="dropdown">
                    <a href="#services" class="dropbtn">Marketing & Bookings</a>
                    <div class="dropdown-content">
                        <a href="#services">Airbnb Optimization</a>
                        <a href="#services">VRBO Marketing</a>
                        <a href="#services">Local Advertising</a>
                    </div>
                </li>
                <li><a href="#contact">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Simplify Your Property Management in Central Florida</h1>
            <p>Expert services for vacation rentals in Orlando, Kissimmee, and beyond.</p>
            <a href="#contact" class="cta-button">Get a Quote</a>
        </div>
    </section>

    <!-- About Us Section -->
    <section id="about" class="about">
        <h2>About Us</h2>
        <p>At Central Florida Property Services, we specialize in managing vacation rentals and properties in Orlando, Kissimmee, and Central Florida. Our dedicated team ensures your properties thrive with top-tier management, cleaning, and marketing services.</p>
        <p>With deep roots in the Central Florida community, we’re committed to delivering stress-free solutions for property owners and exceptional experiences for guests.</p>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-grid">
            <div class="service-item">
                <h3>Property Management</h3>
                <p>Comprehensive management for your vacation rentals, including guest support, bookings, and maintenance across Central Florida.</p>
            </div>
            <div class="service-item">
                <h3>Full-Service Cleanings</h3>
                <p>Impeccable cleaning services to keep your Orlando and Kissimmee properties spotless and guest-ready.</p>
            </div>
            <div class="service-item">
                <h3>Marketing & Bookings</h3>
                <p>Maximize rental income with targeted marketing on Airbnb, VRBO, and Central Florida travel platforms.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <form id="contact-form" action="https://formspree.io/f/your-formspree-endpoint" method="POST">
            <input type="text" id="name" name="name" placeholder="Your Name" required>
            <input type="email" id="email" name="email" placeholder="Your Email" required>
            <select id="service" name="service" required>
                <option value="" disabled selected>Select a Service</option>
                <option value="property-management">Property Management</option>
                <option value="cleaning">Full-Service Cleanings</option>
                <option value="marketing">Marketing & Bookings</option>
            </select>
            <textarea id="message" name="message" placeholder="Tell us about your property needs" required></textarea>
            <button type="submit">Send Message</button>
        </form>
        <p id="form-message"></p>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2025 Central Florida Property Services. All rights reserved.</p>
        <p>Kissimmee, FL | info@centralfloridapropertyservices.com | (407) 555-5678</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

/* Reset default styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Roboto', Arial, sans-serif;
    line-height: 1.6;
    color: #333;
    scroll-behavior: smooth;
    background: #ffffff; /* Clean white background */
}

/* Header */
header {
    background: #1a2b4d; /* Navy blue */
    color: white;
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.logo {
    font-size: 1.8rem;
    font-weight: 700;
    color: #d4a017; /* Gold */
}

.logo-img {
    max-height: 50px;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 30px;
    align-items: center;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1rem;
    font-weight: 400;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: #d4a017; /* Gold on hover */
}

/* Dropdown Menu */
.dropdown {
    position: relative;
}

.dropbtn {
    cursor: pointer;
}

.dropdown-content {
    display: none;
    position: absolute;
    background: #1a2b4d; /* Navy blue */
    min-width: 200px;
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    z-index: 1;
    border-radius: 5px;
    top: 100%;
    left: 0;
}

.dropdown-content a {
    color: white;
    padding: 12px 16px;
    display: block;
    font-size: 0.9rem;
    text-decoration: none;
}

.dropdown-content a:hover {
    background: #2d4373; /* Lighter navy */
    color: #d4a017;
}

.dropdown:hover .dropdown-content {
    display: block;
}

/* Hero Section */
.hero {
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://source.unsplash.com/random/1200x600/?kissimmee') no-repeat center/cover;
    color: white;
    text-align: center;
    padding: 120px 20px;
}

.hero-content {
    max-width: 800px;
    margin: 0 auto;
}

.hero h1 {
    font-size: 2.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
}

.hero p {
    font-size: 1.2rem;
    font-weight: 300;
    margin-bottom: 2rem;
}

.cta-button {
    background: #d4a017; /* Gold */
    color: #1a2b4d; /* Navy text */
    padding: 12px 30px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: 600;
    transition: background 0.3s;
}

.cta-button:hover {
    background: #b38712; /* Darker gold */
}

/* About Section */
.about {
    padding: 60px 20px;
    max-width: 1200px;
    margin: 0 auto;
    text-align: center;
    background: #f8fafc;
}

.about h2 {
    font-size: 2rem;
    font-weight: 700;
    color: #1a2b4d;
    margin-bottom: 1.5rem;
}

.about p {
    font-size: 1rem;
    font-weight: 300;
    max-width: 800px;
    margin: 0 auto 1rem;
}

/* Services Section */
.services {
    padding: 60px 20px;
    max-width: 1200px;
    margin: 0 auto;
    text-align: center;
}

.services h2 {
    font-size: 2rem;
    font-weight: 700;
    color: #1a2b4d;
    margin-bottom: 2rem;
}

.service-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
}

.service-item {
    background: white;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.service-item:hover {
    transform: translateY(-5px);
}

.service-item h3 {
    font-size: 1.5rem;
    font-weight: 600;
    color: #1a2b4d;
    margin-bottom: 1rem;
}

.service-item p {
    font-size: 0.9rem;
    font-weight: 300;
}

/* Contact Section */
.contact {
    background: #f1f5f9;
    padding: 60px 20px;
    text-align: center;
}

.contact h2 {
    font-size: 2rem;
    font-weight: 700;
    color: #1a2b4d;
    margin-bottom: 2rem;
}

#contact-form {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 15px;
}

#contact-form input,
#contact-form select,
#contact-form textarea {
    padding: 12px;
    border: 1px solid #d1d5db;
    border-radius: 5px;
    font-size: 0.9rem;
    background: white;
}

#contact-form select {
    appearance: none;
    background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="12" height="6"><path fill="#1a2b4d" d="M0 0l6 6 6-6H0z"/></svg>') no-repeat right 10px center;
    background-size: 12px;
}

#contact-form textarea {
    height: 150px;
}

#contact-form button {
    background: #d4a017;
    color: #1a2b4d;
    padding: 12px;
    border: none;
    border-radius: 5px;
    font-size: 0.9rem;
    font-weight: 600;
    cursor: pointer;
    transition: background 0.3s;
}

#contact-form button:hover {
    background: #b38712;
}

#form-message {
    margin-top: 1.5rem;
    color: #15803d;
    font-size: 0.9rem;
}

/* Footer */
footer {
    background: #1a2b4d;
    color: white;
    text-align: center;
    padding: 20px;
}

footer p {
    font-size: 0.9rem;
    font-weight: 300;
    margin: 5px 0;
}

/* Responsive Design */
@media (max-width: 768px) {
    .hero h1 {
        font-size: 2rem;
    }

    .hero p {
        font-size: 1rem;
    }

    nav ul {
        flex-direction: column;
        gap: 15px;
    }

    .dropdown-content {
        position: static;
        box-shadow: none;
        background: #2d4373;
    }

    .service-item {
        padding: 20px;
    }
}

document.getElementById('contact-form').addEventListener('submit', function(e) {
    e.preventDefault();
    
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const service = document.getElementById('service').value;
    const message = document.getElementById('message').value;
    const formMessage = document.getElementById('form-message');

    // Simulate form submission (Formspree handles actual submission)
    formMessage.textContent = `Thank you, ${name}! We'll respond soon about your ${service.replace('-', ' ')} inquiry.`;
    formMessage.style.color = '#15803d';

    // Log submission for testing
    const submission = { name, email, service, message, date: new Date().toISOString() };
    console.log('Form Submission:', submission);

    // Clear form
    this.reset();
});

// Smooth scrolling for navigation links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});
