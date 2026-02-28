---
layout: col-sidebar
title: OWASP JIS University
tags: OWASP-JISU
region: Asia
country: India
meetup-group: owasp-jisu
---

<style>
  /* Container Styles */
  .owasp-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }

  /* Hero Image */
  .hero-image {
    width: 100%;
    max-width: 100%;
    height: auto;
    border-radius: 12px;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.15);
    margin-bottom: 30px;
    display: block;
  }

  /* Notice Card */
  .notice-card {
    background: linear-gradient(135deg, #fff5f5 0%, #ffe8e8 100%);
    border-left: 5px solid #d32f2f;
    border-radius: 10px;
    padding: 25px 30px;
    margin: 30px 0;
    box-shadow: 0 4px 12px rgba(211, 47, 47, 0.1);
  }

  .notice-card .notice-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: #d32f2f;
    text-align: center;
    margin-bottom: 15px;
  }

  .notice-card .notice-content {
    color: #333;
    line-height: 1.7;
    text-align: center;
    font-size: 1rem;
  }

  .notice-content strong {
    color: #d32f2f;
  }

  /* Welcome Section */
  .welcome-section {
    background: linear-gradient(135deg, #f8f9fa 0%, #e3f2fd 100%);
    border-radius: 12px;
    padding: 35px;
    margin: 30px 0;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
  }

  .welcome-section h2 {
    color: #1565c0;
    font-size: 2rem;
    margin-bottom: 15px;
    border-bottom: 3px solid #1565c0;
    padding-bottom: 10px;
    display: inline-block;
  }

  .welcome-section p {
    font-size: 1.1rem;
    line-height: 1.8;
    color: #424242;
  }

  /* Mission Section */
  .mission-section {
    margin: 40px 0;
  }

  .mission-section h2 {
    color: #2e7d32;
    font-size: 1.8rem;
    margin-bottom: 20px;
    text-align: center;
  }

  .mission-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
    margin-top: 25px;
  }

  .mission-item {
    background: #ffffff;
    border-left: 4px solid #2e7d32;
    border-radius: 8px;
    padding: 20px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .mission-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 20px rgba(46, 125, 50, 0.2);
  }

  .mission-item::before {
    content: "✓";
    display: inline-block;
    width: 25px;
    height: 25px;
    background: #2e7d32;
    color: white;
    border-radius: 50%;
    text-align: center;
    line-height: 25px;
    margin-right: 12px;
    font-weight: bold;
  }

  /* Member Section */
  .member-section {
    background: linear-gradient(135deg, #e8f5e9 0%, #c8e6c9 100%);
    border-radius: 12px;
    padding: 40px 30px;
    margin: 40px 0;
    text-align: center;
  }

  .member-section h2 {
    color: #2e7d32;
    font-size: 2rem;
    margin-bottom: 25px;
  }

  .join-btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 16px 40px;
    background: linear-gradient(135deg, #007bff 0%, #0056b3 100%);
    color: #fff;
    text-decoration: none;
    border-radius: 50px;
    font-weight: 700;
    font-size: 1.1rem;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(0, 123, 255, 0.3);
    border: none;
  }

  .join-btn:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 25px rgba(0, 123, 255, 0.4);
    background: linear-gradient(135deg, #0056b3 0%, #003d82 100%);
  }

  .join-btn .owasp-logo {
    width: 28px;
    height: 28px;
    margin-right: 10px;
    filter: brightness(0) invert(1);
  }

  /* Info Box */
  .info-box {
    background: #fff3e0;
    border-left: 4px solid #ff9800;
    border-radius: 8px;
    padding: 20px;
    margin: 25px 0;
    text-align: center;
    font-size: 1.05rem;
    color: #e65100;
    font-weight: 500;
  }

  /* Bengali Welcome */
  .bengali-welcome {
    background: linear-gradient(135deg, #fce4ec 0%, #f8bbd0 100%);
    border-radius: 12px;
    padding: 30px;
    margin: 30px 0;
    text-align: center;
    box-shadow: 0 4px 12px rgba(233, 30, 99, 0.15);
  }

  .bengali-welcome p {
    font-size: clamp(1.4rem, 5vw, 2.2rem);
    color: #c2185b;
    font-weight: 700;
    margin: 0;
    line-height: 1.4;
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .owasp-container {
      padding: 0 15px;
    }

    .notice-card {
      padding: 20px 15px;
    }

    .notice-card .notice-title {
      font-size: 1.2rem;
    }

    .notice-card .notice-content {
      font-size: 0.95rem;
    }

    .welcome-section {
      padding: 25px 20px;
    }

    .welcome-section h2 {
      font-size: 1.5rem;
    }

    .welcome-section p {
      font-size: 1rem;
    }

    .mission-section h2 {
      font-size: 1.5rem;
    }

    .mission-grid {
      grid-template-columns: 1fr;
      gap: 15px;
    }

    .mission-item {
      padding: 15px;
    }

    .member-section {
      padding: 30px 20px;
    }

    .member-section h2 {
      font-size: 1.6rem;
    }

    .join-btn {
      padding: 14px 30px;
      font-size: 1rem;
      width: 100%;
      max-width: 300px;
    }

    .info-box {
      padding: 15px;
      font-size: 0.95rem;
    }

    .bengali-welcome {
      padding: 20px 15px;
    }
  }

  @media (max-width: 480px) {
    .hero-image {
      border-radius: 8px;
    }

    .notice-card .notice-title {
      font-size: 1.1rem;
    }

    .welcome-section h2 {
      font-size: 1.3rem;
    }

    .mission-section h2 {
      font-size: 1.3rem;
    }

    .member-section h2 {
      font-size: 1.4rem;
    }
  }
</style>

<div class="owasp-container">
  <img src="https://raw.githubusercontent.com/OWASP/www-chapter-jis-university-student-chapter/main/assets/images/OWASP%20JISU.jpg" alt="OWASP JIS University" class="hero-image">

  <div class="notice-card">
    <div class="notice-title">⚠️ IMPORTANT NOTICE</div>
    <div class="notice-content">
      <strong>OWASP website migration is currently in progress by the OWASP team.</strong><br><br>
      This chapter page is part of the legacy GitHub-hosted site.<br>
      The <strong>new official OWASP chapter website</strong> will be available in the coming months.<br><br>
      Until then, please <strong>join our WhatsApp community</strong> to stay updated on events, sessions, and announcements.
    </div>
  </div>

  <div class="welcome-section">
    <h2>Welcome to OWASP JIS University</h2>
    <p>
      OWASP JIS University is a <strong>student-led cybersecurity community</strong> affiliated with the <strong>Open Worldwide Application Security Project (OWASP)</strong>. We are dedicated to <strong>building a security-first mindset</strong> through hands-on <strong>workshops, CTFs, hackathons, and research</strong> in cybersecurity and application security.
    </p>
  </div>

  <div class="mission-section">
    <h2>🥷 Our Mission</h2>
    <div class="mission-grid">
      <div class="mission-item">
        Promote <strong>secure coding practices</strong> among students.
      </div>
      <div class="mission-item">
        Encourage <strong>ethical hacking</strong> and <strong>security research</strong>.
      </div>
      <div class="mission-item">
        Collaborate on <strong>open-source security projects</strong>.
      </div>
      <div class="mission-item">
        Organize <strong>events, workshops, and hackathons</strong> on cybersecurity.
      </div>
      <div class="mission-item">
        Contribute to <strong>OWASP global initiatives</strong>.
      </div>
      <div class="mission-item">
        Foster a <strong>collaborative learning environment</strong> for cybersecurity enthusiasts.
      </div>
    </div>
  </div>

  <div class="member-section">
    <h2>🧑🏻‍💻 Become a Member</h2>
    <a href="https://chat.whatsapp.com/KaDR5HpXz2v7VVjvBIk61Y" target="_blank" rel="noopener noreferrer" class="join-btn" title="Join OWASP JISU" aria-label="Join OWASP JISU">
      Join OWASP JISU
    </a>
  </div>

  <div class="info-box">
    💡 OWASP chapters are open to everyone—students, professionals, and cybersecurity enthusiasts!
  </div>

  <div class="bengali-welcome">
    <p>OWASP JIS University Student Chapter-এ আপনাকে স্বাগতম 🙏</p>
  </div>
</div>
