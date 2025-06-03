<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Central Florida Property Services - Property Management, Full-Service Cleanings, and Marketing for Vacation Rentals in Orlando and surrounding areas.">
    <meta name="keywords" content="property management, vacation rental cleaning, Orlando property services, Central Florida rentals">
    <title>Central Florida Property Services</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <div class="logo">Central Florida Property Services</div>
            <ul>
                <liertown, FL 34747</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Premier Property Services in Central Florida</h1>
        <p>Expert property management, cleaning, and marketing for your vacation rentals in Orlando, Kissimmee, and beyond.</p>
        <a href="#contact" class="cta-button">Request a Quote</a>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-grid">
            <div class="service-item">
                <h3>Property Management</h3>
                <p>Comprehensive management for vacation rentals, including guest communication, bookings, and maintenance in Central Florida.</p>
            </div>
            <div class="service-item">
                <h3>Full-Service Cleanings</h3>
                <p>Top-quality cleaning services to keep your properties spotless and guest-ready in Orlando and surrounding areas.</p>
            </div>
            <div class="service-item">
                <h3>Marketing & Bookings</h3>
                <p>Boost your rental income with targeted marketing on platforms like Airbnb, VRBO, and local Central Florida channels.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Get in Touch</h2>
        <form id="contact-form">
            <input type="text" id="name" placeholder="Your Name" required>
            <input type="email" id="email" placeholder="Your Email" required>
            <textarea id="message" placeholder="Tell us about your property needs" required></textarea>
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
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
}

/* Header */
header {
    background: #004aad; /* Central Florida-inspired blue */
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
    font-size: 1.5rem;
    font-weight: bold;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1rem;
}

nav ul li a:hover {
    text-decoration: underline;
}

/* Hero Section */
.hero {
    background: url('https://source.unsplash.com/random/1200x400/?central-florida') no-repeat center/cover;
    color: white;
    text-align: center;
    padding: 100px 20px;
}

.hero h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.cta-button {
    background: #ff6200; /* Orange to evoke Florida’s vibrancy */
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
}

.cta-button:hover {
    background: #e55a00;
}

/* Services Section */
.services {
    padding: 50px 20px;
    max-width: 1200px;
    margin: 0 auto;
    text-align: center;
}

.services h2 {
    font-size: 2rem;
    margin-bottom: 2rem;
}

.service-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.service-item {
    background: #f9f9f9;
    padding: 20px;
    border-radius: 5px;
}

.service-item h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
}

/* Contact Section */
.contact {
    background: #f4f4f4;
    padding: 50px 20px;
    text-align: center;
}

.contact h2 {
    font-size: 2rem;
    margin-bottom: 2rem;
}

#contact-form {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 10px;
}

#contact-form input,
#contact-form textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 1rem;
}

#contact-form textarea {
    height: 150px;
}

#contact-form button {
    background: #004aad;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

#contact-form button:hover {
    background: #003a8c;
}

#form-message {
    margin-top: 1rem;
    color: green;
}

/* Footer */
footer {
    background: #333;
    color: white;
    text-align: center;
    padding: 20px;
}

footer p {
    margin: 5px 0;
}

/* Responsive Design */
@media (max-width: 768px) {
    .hero h1 {
        font-size: 2rem;
    }

    nav ul {
        flex-direction: column;
        gap: 10px;
    }
}
