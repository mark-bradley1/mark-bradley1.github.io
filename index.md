---
layout: default
title: Home
---

<section class="hero fade-in">
  <h1>Hi, I'm Mark</h1>
  <p>
    Full-stack developer building clean, scalable web applications with Java, Spring Boot, and React.
  </p>

  <div class="hero-actions">
    <a href="#projects" class="button">View Projects</a>
    <a href="#contact" class="button">Contact Me</a>
  </div>
</section>

<section class="fade-in">
  <h2>What I Do</h2>

  <div class="projects-grid">
    <div class="card">
      <h3>Full Stack Development</h3>
      <p>Building scalable applications using Spring Boot, REST APIs, and React.</p>
    </div>

    <div class="card">
      <h3>Backend Systems</h3>
      <p>Designing clean APIs, database models, and secure authentication flows.</p>
    </div>

    <div class="card">
      <h3>Frontend UI</h3>
      <p>Creating responsive, user-friendly interfaces with modern design.</p>
    </div>
  </div>
</section>

<section id="projects" class="fade-in">
  <h2>Projects</h2>

  <div class="projects-grid">

    <div class="project-card">
      <div class="project-content">
        <h3>Price Comparison App</h3>
        <p>
          A full-stack app that compares grocery prices across stores using real-time API data.
        </p>

        <ul class="project-tags">
          <li>Java</li>
          <li>JavaScript</li>
          <li>HTML</li>
          <li>CSS</li>
          <li>Spring Boot</li>
          <li>React</li>
          <li>MySQL</li>
        </ul>
      </div>

      <div class="project-footer">
        <a href="https://github.com/mark-bradley1/Unit2-Final-Project-Price-Comparison" class="button small secondary" target="_blank">GitHub</a>
      </div>
    </div>

  </div>
</section>

<section id="contact" class="fade-in contact-section">
  <h2>Contact Me</h2>
  <p>I'd love to hear from you! Fill out the form below or reach me directly via email.</p>

  <form action="https://formspree.io/f/mbdpaprb" method="POST" class="contact-form">
    <div class="form-group">
      <input type="text" name="name" placeholder="Your Name" required>
    </div>
    <div class="form-group">
      <input type="email" name="_replyto" placeholder="Your Email" required>
    </div>
    <div class="form-group">
      <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
    </div>
    <button type="submit" class="button">Send Message</button>
  </form>

  <p class="contact-alt">
    Or email me directly at 
    <a href="mailto:mbradle15@gmail.com">mbradle15@gmail.com</a>
  </p>
</section>
