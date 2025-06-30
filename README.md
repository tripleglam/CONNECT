# CONNECT
A website that helps you CONNECT with nonprofit organizations 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Connect with Nonprofits</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Connect with Nonprofits</h1>
    <p>Find and reach out to nonprofit organizations making a difference.</p>
  </header>

  <main class="org-list">
    <!-- Example Nonprofit Card -->
    <div class="org-card">
      <h2>Green Earth Foundation</h2>
      <p>Dedicated to reforestation and climate action around the globe.</p>
      <button onclick="openContactForm('Green Earth Foundation')">Contact</button>
    </div>

    <div class="org-card">
      <h2>Hope for All</h2>
      <p>Provides shelter, education, and support for homeless youth.</p>
      <button onclick="openContactForm('Hope for All')">Contact</button>
    </div>

    <div class="org-card">
      <h2>FoodShare Network</h2>
      <p>Combats hunger by connecting surplus food with people in need.</p>
      <button onclick="openContactForm('FoodShare Network')">Contact</button>
    </div>
  </main>

  <!-- Contact Form Modal -->
  <div id="contactModal" class="modal">
    <div class="modal-content">
      <span class="close" onclick="closeContactForm()">&times;</span>
      <h2>Contact <span id="orgName"></span></h2>
      <form onsubmit="submitForm(event)">
        <label for="name">Your Name:</label>
        <input type="text" id="name" required />
        <label for="email">Your Email:</label>
        <input type="email" id="email" required />
        <label for="message">Message:</label>
        <textarea id="message" rows="4" required></textarea>
        <button type="submit">Send Message</button>
      </form>
    </div>
  </div>

  <footer>
    <p>&copy; 2025 Connect with Nonprofits</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
