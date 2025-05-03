# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>GizmoHub</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <div class="logo">GizmoHub</div>
    <nav>
      <ul class="navbar">
        <li><a href="#home">Home</a></li>
        <li><a href="#gadgets">Gadgets</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#team">Team</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>
  <section id="home" class="section hero">
    <h1>Innovative Tech for Modern Life</h1>
    <p>Upgrade your world with GizmoHub's top gadgets</p>
  </section>
  <section id="gadgets" class="section gadgets">
    <h2>Featured Products</h2>
    <div class="gadget-grid">
      <div class="gadget-card">
        <img src="Screenshot 2025-05-03 144511.png" alt="Wireless Earbuds">
        <h3>Wireless Earbuds</h3>
      </div>
      <div class="gadget-card">
        <img src="Screenshot 2025-05-03 144517.png" alt="Smartwatch">
        <h3>Smartwatch Pro</h3>
      </div>
      <div class="gadget-card">
        <img src="Screenshot 2025-05-03 144524.png" alt="Bluetooth Speaker">
        <h3>360° Bluetooth Speaker</h3>
      </div>
    </div>
  </section>
  <section id="services" class="section services">
    <h2>Our Services</h2>
    <div class="service-grid">
      <div class="service-box">
        <img src="download (1).png" alt="Shipping Icon">
        <h3>Fast Shipping</h3>
        <p>Get your gadgets delivered within 24–48 hours across major cities.</p>
      </div>
      <div class="service-box">
        <img src="download (16).jpg" alt="Support Icon">
        <h3>24/7 Support</h3>
        <p>Our dedicated team is available around the clock for your queries.</p>
      </div>
      <div class="service-box">
        <img src="images.png" alt="Secure Payment Icon">
        <h3>Secure Payments</h3>
        <p>Multiple payment methods with 256-bit encryption security.</p>
      </div>
    </div>
  </section>
  <section id="team" class="section team">
    <h2>Meet the Team</h2>
    <div class="team-grid">
      <div class="team-member">
        <img src="Screenshot 2025-05-03 145645.png" alt="CEO">
        <h4>Riya Mehra</h4>
        <p>Founder & CEO - Tech visionary and innovation leader.</p>
      </div>
      <div class="team-member">
        <img src="Screenshot 2025-05-03 145651.png" alt="Designer">
        <h4>Aditya Singh</h4>
        <p>UI/UX Lead - Creating clean and powerful user experiences.</p>
      </div>
      <div class="team-member">
        <img src="Screenshot 2025-05-03 145659.png" alt="Tech Lead">
        <h4>Priya Kapoor</h4>
        <p>Tech Lead - Architect behind every product you trust.</p>
      </div>
    </div>
  </section>
  <section id="contact" class="section contact">
    <h2>Contact Us</h2>
    <div class="contact-grid">
      <div class="contact-box">
        <h4>Email</h4>
        <p>support@gizmohub.com</p>
      </div>
      <div class="contact-box">
        <h4>Phone</h4>
        <p>+91 800-123-4567</p>
      </div>
      <div class="contact-box">
        <h4>Location</h4>
        <p>GizmoHub HQ, Bengaluru, India</p>
      </div>
    </div>
  </section>
  <footer>
    <div class="social-links">
      <a href="#">Facebook</a> | 
      <a href="#">Instagram</a> | 
      <a href="#">YouTube</a>
    </div>
    <p>&copy; 2025 GizmoHub. All rights reserved.</p>
  </footer>
</body>
</html>

```
style.css
```
body {
  margin: 0;
  font-family: 'Helvetica Neue', sans-serif;
  background-color: #f4f4f4;
  color: #333;
}

header {
  background-color: #1a1a1a;
  color: white;
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.navbar {
  display: flex;
  list-style: none;
  gap: 1.5rem;
}

.navbar a {
  color: white;
  text-decoration: none;
  transition: color 0.3s ease;
}

.navbar a:hover {
  color: #00bcd4;
}

.section {
  padding: 4rem 2rem;
  text-align: center;
}

.hero {
  background: linear-gradient(to right, #00bcd4, #2196f3);
  color: white;
  padding: 5rem 2rem;
}

.gadget-grid {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 2rem;
  margin-top: 2rem;
}

.gadget-card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  width: 250px;
  padding: 1rem;
  transition: transform 0.3s ease;
}

.gadget-card:hover {
  transform: translateY(-5px);
}

.gadget-card img {
  width: 100%;
  border-radius: 6px;
}
.service-grid, .team-grid {
  display: flex;
  gap: 2rem;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 2rem;
}

.service-box, .team-member {
  background: white;
  padding: 1.5rem;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  width: 250px;
  text-align: center;
  transition: transform 0.3s ease;
}

.service-box:hover, .team-member:hover {
  transform: translateY(-5px);
}

.service-box img,
.team-member img {
  width: 60px;
  height: 60px;
  margin-bottom: 1rem;
  border-radius: 50%;
  object-fit: cover;
}

.team-member h4 {
  margin: 0.5rem 0 0.3rem;
}
.contact-grid {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
  margin-top: 2rem;
}

.contact-box {
  background: white;
  padding: 1.5rem 2rem;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  width: 100%;
  max-width: 400px;
  text-align: center;
}

.contact-box h4 {
  margin-bottom: 0.5rem;
  color: #00bcd4;
}

footer {
  background-color: #1a1a1a;
  color: white;
  text-align: center;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.social-links {
  margin-bottom: 1rem;
}

.social-links a {
  color: #ccc;
  margin: 0 0.5rem;
  text-decoration: none;
}

.social-links a:hover {
  color: white;
}
@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    gap: 1rem;
  }

  .gadget-grid,
  .service-grid,
  .team-grid {
    flex-direction: column;
    align-items: center;
  }
}

```


## OUTPUT
![Screenshot 2025-05-03 150017](https://github.com/user-attachments/assets/22f9f182-e2aa-4b89-874b-31eb150efb39)
![Screenshot 2025-05-03 150032](https://github.com/user-attachments/assets/78f77198-4bdc-4772-87ce-23262cbd6aca)
![Screenshot 2025-05-03 150057](https://github.com/user-attachments/assets/e0550aa1-e9d9-401f-a2c3-1b5047202837)
![Screenshot 2025-05-03 150112](https://github.com/user-attachments/assets/8f289dca-68fa-430a-b760-6514742f0e4e)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
