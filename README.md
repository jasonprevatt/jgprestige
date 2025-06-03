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
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Elevate Your Central Florida Properties</h1>
            <p>Premier property management, cleaning, and marketing services for vacation rentals in Orlando, Kissimmee, and beyond.</p>
            <a href="#contact" class="cta-button">Request a Quote</a>
        </div>
    </section>

    <!-- About Us Section -->
    <section id="about" class="about">
        <h2>About Us</h2>
        <p>We are Central Florida Property Services, your trusted partner in managing vacation rentals and properties in Orlando, Kissimmee, and surrounding areas. With a passion for hospitality and local expertise, we deliver exceptional property management, cleaning, and marketing to maximize your rental income and guest satisfaction.</p>
        <p>Our mission is to make property ownership stress-free while ensuring guests enjoy unforgettable stays in Central Florida’s vibrant communities.</p>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-grid">
            <div class="service-item">
                <h3>Property Management</h3>
                <p>Comprehensive management for vacation rentals, including guest communication, bookings, and maintenance across Central Florida.</p>
            </div>
            <div class="service-item">
                <h3>Full-Service Cleanings</h3>
                <p>Impeccable cleaning services to keep your Orlando and Kissimmee properties spotless and guest-ready.</p>
            </div>
            <div class="service-item">
                <h3>Marketing & Bookings</h3>
                <p>Boost your rental income with targeted marketing on Airbnb, VRBO, and Central Florida travel platforms.</p>
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
}

/* Header */
header {
    background: #1e3a8a; /* Clean, modern blue */
    color: white;
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
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
}

.logo-img {
    max-height: 50px;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 30px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.1rem;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: #f97316; /* Modern orange accent */
}

/* Hero Section */
.hero {
    background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://source.unsplash.com/random/1200x600/?orlando') no-repeat center/cover;
    color: white;
    text-align: center;
    padding: 140px 20px;
}

.hero-content {
    max-width: 800px;
    margin: 0 auto;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 1.5rem;
    font-weight: 700;
}

.hero p {
    font-size: 1.3rem;
    margin-bottom: 2rem;
}

.cta-button {
    background: #f97316;
    color: white;
    padding: 12px 30px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: 600;
    transition: background 0.3s;
}

.cta-button:hover {
    background: #ea580c;
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
    font-size: 2.2rem;
    margin-bottom: 1.5rem;
    color: #1e3a8a;
}

.about p {
    font-size: 1.1rem;
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
    font-size: 2.2rem;
    margin-bottom: 2rem;
    color: #1e3a8a;
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
    font-shape: square;
    font-size: 1.6rem;
    margin-bottom: 1rem;
    color: #1e3a8a;
}

.service-item p {
    font-size: 1rem;
}

/* Contact Section */
.contact {
    background: #f1f5f9;
    padding: 60px 20px;
    text-align: center;
}

.contact h2 {
    font-size: 2.2rem;
    margin-bottom: 2rem;
    color: #1e3a8a;
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
    font-size: 1rem;
    background: white;
}

#contact-form select {
    appearance: none;
    background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="12" height="6"><path d="M0 0l6 6 6-6H0z"/></svg>') no-repeat right 10px center;
    background-size: 12px;
}

#contact-form textarea {
    height: 160px;
}

#contact-form button {
    background: #1e3a8a;
    color: white;
    padding: 12px;
    border: none;
    border-radius: 5px;
    font-size: 1rem;
    cursor: pointer;
    transition: background 0.3s;
}

#contact-form button:hover {
    background: #1e3a8a;
}

#form-message {
    margin-top: 1.5rem;
    color: #15803d;
    font-size: 1rem;
}

/* Footer */
footer {
    background: #1e3a8a;
    color: white;
    text-align: center;
    padding: 25px;
}

footer p {
    margin: 8px 0;
    font-size: 0.9rem;
}

/* Responsive Design */
@media (max-width: 768px) {
    .hero h1 {
        font-size: 2.2rem;
    }

    .hero p {
        font-size: 1.1rem;
    }

    nav ul {
        flex-direction: column;
        gap: 15px;
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
