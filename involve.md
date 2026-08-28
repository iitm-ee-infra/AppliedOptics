---
layout: single
title: "Contact Us"
---

<!-- Plain Text Title Block (Centered) -->
<div class="container" style="padding-top: 20px; padding-bottom: 20px; text-align: center;">
  <h1 style="color: #1a365d; font-family: 'Calibri', sans-serif; font-weight: bold; font-size: 3rem; margin-bottom: 0;">
    Contact Us
  </h1>
  <hr style="border-top: 2px solid #1a365d; margin: 15px auto 0 auto; width: 50%;">
</div>

<!-- CSS Styling for Contact Layout -->
<style>
  .contact-container {
    max-width: 900px;
    margin: 0 auto;
    padding: 20px 0;
    font-family: 'Calibri', sans-serif;
  }

  .contact-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 40px;
    margin-bottom: 30px;
  }

  .contact-column {
    flex: 1;
    min-width: 300px;
  }

  .contact-card {
    background: #f8fafc;
    border: 1px solid #e2e8f0;
    border-left: 4px solid #1a365d;
    border-radius: 8px;
    padding: 25px;
    margin-bottom: 25px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.02);
  }

  .card-title {
    color: #1a365d;
    font-size: 1.4rem;
    font-weight: bold;
    margin-top: 0;
    margin-bottom: 15px;
  }

  .contact-details {
    color: #334155;
    font-size: 16px;
    line-height: 1.6;
    margin: 0;
  }

  .contact-item {
    margin-bottom: 12px;
    display: flex;
    align-items: flex-start;
  }

  .contact-item i {
    color: #1a365d;
    font-size: 1.2rem;
    margin-right: 12px;
    margin-top: 4px;
    width: 20px;
    text-align: center;
  }

  .contact-item a {
    color: #0077b5;
    text-decoration: none;
    font-weight: bold;
  }

  .contact-item a:hover {
    color: #38bdf8;
    text-decoration: underline;
  }

  /* Centered Responsive Map Wrapper Styling */
  .map-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    margin: 0 auto;
  }

  .map-wrapper iframe {
    width: 100%;
    max-width: 800px;
    height: 450px;
    border-radius: 8px;
    border: 1px solid #e2e8f0;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
  }
</style>

<div class="container">
  <div class="contact-container">

    <div class="contact-grid">

      <!-- LEFT COLUMN: ADDRESS & LAB LOCATION -->
      <div class="contact-column">
        <div class="contact-card">
          <h3 class="card-title">Laboratory Location</h3>
          <div class="contact-details">
            <div class="contact-item">
              <i class="fa fa-university"></i>
              <span>
                <strong>Applied Optics Group</strong><br>
                Department of Electrical Engineering<br>
                Indian Institute of Technology Madras (IITM)<br>
                Chennai, Tamil Nadu - 600036, India
              </span>
            </div>
            <div class="contact-item">
              <i class="fa fa-building"></i>
              <span>Room No: ESB:  335-B</span>
            </div>
          </div>
        </div>
      </div>

      <!-- RIGHT COLUMN: ADVISOR CONTACT DETAILS -->
      <div class="contact-column">
        <div class="contact-card">
          <h3 class="card-title">Group Advisor</h3>
          <div class="contact-details">
            <p style="font-weight: bold; font-size: 1.1rem; margin-top: 0; margin-bottom: 5px; color: #1a365d;">
              Dr. Shanti Bhattacharya
            </p>
            <p style="color: #64748b; margin-top: 0; margin-bottom: 15px; font-size: 14px;">
              Head of the department, Department of Electrical Engineering
            </p>

            <div class="contact-item">
              <i class="fa fa-envelope"></i>
              <span>Email: <a href="mailto:shanti@ee.iitm.ac.in">shanti@ee.iitm.ac.in</a></span>
            </div>
            <div class="contact-item">
              <i class="fa fa-linkedin-square"></i>
              <span>LinkedIn: <a href="https://www.linkedin.com/in/dr-shanti-bhattacharya-069210209/" target="_blank">View Profile</a></span>
            </div>
          </div>
        </div>
      </div>

    </div>

    <!-- MAP SECTION ROW -->
    <h2 style="color: #1a365d; font-family: 'Calibri', sans-serif; font-weight: bold; font-size: 1.6rem; border-bottom: 2px solid #1a365d; padding-bottom: 8px; margin-bottom: 20px; text-align: center;">
      Find Us on Campus
    </h2>

    <div class="map-wrapper">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d7775.461804243976!2d80.2301135!3d12.989055699999994!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3a525d806fcc990b%3A0x1d01b71b29fcc0fc!2sCSD%20Building!5e0!3m2!1sen!2sin!4v1787912185394!5m2!1sen!2sin" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="strict-origin-when-cross-origin"></iframe>
    </div>

    <div style="text-align: center; margin-top: 15px;">
      <a href="https://maps.app.goo.gl/GiTU9be4koVhDRbi9" target="_blank" style="color: #0077b5; font-weight: bold; text-decoration: none; font-size: 15px;">
        <i class="fa fa-map-marker" style="margin-right: 5px;"></i> Can't see the map? Open directly in Google Maps &raquo;
      </a>
    </div>

  </div>
</div>
