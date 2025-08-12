<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Sam Adedams — Web Developer · Graphic Designer · Brand Marketer</title>
<style>
  body {font-family: 'Times New Roman', serif; margin:0; padding:0; background:linear-gradient(to bottom, #0d1b4c, #d4af37); color:white;}
  section {padding:50px 20px;}
  h1 {text-align:center; color:gold; font-size:3em; margin-top:40px;}
  h2 {text-transform:uppercase; border-bottom:3px solid gold; display:inline-block; padding-bottom:5px;}
  .btn {background:gold; color:#0d1b4c; padding:10px 20px; border:none; cursor:pointer; font-weight:bold; border-radius:5px;}
  form {background:rgba(255,255,255,0.1); padding:20px; border-radius:10px;}
  input, textarea, select {width:100%; padding:10px; margin-bottom:15px; border-radius:5px; border:none;}
  label {font-weight:bold;}
  footer {text-align:center; padding:20px; background:#0d1b4c;}

  /* Animation */
  @keyframes fadeInUp {
    0% {opacity: 0; transform: translateY(20px);}
    100% {opacity: 1; transform: translateY(0);}
  }
  .animated-intro {
    text-align:center;
    animation: fadeInUp 2s ease-in-out;
  }
</style>
</head>
<body>
<header>
  <h1>SAM ADEDAMS</h1>
  <p class="animated-intro">Web Developer · Graphic Designer · Brand Marketer</p>
</header>

<section id="home">
  <h2>Home</h2>
  <p>Welcome! I am Sam Adedams, a creative professional with expertise in web development, graphic design, and brand marketing. I deliver visually stunning, functional, and growth-driven solutions.</p>
</section>

<section id="about">
  <h2>About</h2>
  <p>I am a multi-disciplinary creative with over four years of professional experience combining technology, design, and marketing. Between 2021 and 2025, I worked with dGlobalGrowthField Tech Hub, where I collaborated with teams to build high-performing websites, craft visual identities for emerging brands, and design user experiences that elevated client engagement. My approach is driven by attention to detail, creativity, and the belief that design and technology must work hand-in-hand to produce results that inspire and convert. Beyond technical execution, I offer strategic insights that help businesses establish a strong presence in competitive markets.</p>
</section>

<section id="services">
  <h2>Services</h2>
  <ul>
    <li><strong>Web Development:</strong> I build responsive, SEO-optimized, and user-friendly websites tailored to your goals.</li>
    <li><strong>Graphic Design:</strong> From logos to full visual identity systems, I create designs that speak to your audience.</li>
    <li><strong>Brand Marketing:</strong> I develop strategies that grow your brand, increase engagement, and boost conversions.</li>
  </ul>
</section>

<section id="experience">
  <h2>Experience</h2>
  <p>Throughout my career, I have developed and launched numerous digital solutions, from small business websites to enterprise-level platforms. At dGlobalGrowthField Tech Hub, I played a key role in scaling client brands by merging design thinking with modern web technologies, resulting in solutions that not only looked professional but also delivered measurable growth. My responsibilities included leading UI/UX projects, creating marketing collateral, optimizing site performance, and mentoring junior designers and developers. These experiences have equipped me with the ability to manage complex projects from concept to launch, ensuring alignment with client goals and market trends.</p>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>Please fill out the form below to get in touch. Purpose of contact is required.</p>
  <form id="contactForm" onsubmit="return handleForm(event)">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" required>
    <label for="email">Email</label>
    <input type="email" id="email" name="email" required>
    <label for="purpose">Purpose of Contact</label>
    <select id="purpose" name="purpose" required>
      <option value="">--Select--</option>
      <option>Hire Me</option>
      <option>Collaboration</option>
      <option>General Inquiry</option>
    </select>
    <label for="message">Message</label>
    <textarea id="message" name="message" required></textarea>
    <button type="submit" class="btn">Send</button>
  </form>
  <p id="response"></p>
</section>

<footer>
  <p>© <span id="year"></span> Sam Adedams | Email: samadedamola4@gmail.com | Phone: +234 903 283 0132</p>
</footer>

<script>
  document.getElementById('year').textContent = new Date().getFullYear();

  function handleForm(e){
    e.preventDefault();
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const purpose = document.getElementById('purpose').value;
    const message = document.getElementById('message').value;
    if(!name || !email || !purpose || !message){
      document.getElementById('response').textContent = 'Please fill all fields.';
      return;
    }
    // Simulated backend process
    document.getElementById('response').textContent = 'Form submitted successfully!';
  }
</script>
</body>
</html>
