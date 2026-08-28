---
layout: single
---

<!-- Title Block -->
<div class="container" style="padding-top: 0px; padding-bottom: 20px; margin-top: -100px; text-align: center;">
  <h1 style="color: #36454f; font-family: 'Calibri', sans-serif; font-weight: bold; font-size: 3rem; margin-bottom: 0;">
    Resources
  </h1>
  <hr style="border-top: 2px solid #1a365d; margin: 15px auto 0 auto; width: 50%;">
</div>

<!-- CSS Styles for Resources List & Added Elements -->
<style>
  .resources-container {
    max-width: 800px;
    margin: 40px auto 30px auto;
    padding: 0 20px;
    font-family: 'Calibri', sans-serif;
  }

  .resources-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .resource-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 20px;
    margin-bottom: 12px;
    background-color: #f8fafc;
    border: 1px solid #e2e8f0;
    border-radius: 6px;
    transition: background-color 0.2s ease;
  }

  .resource-item:hover {
    background-color: #f1f5f9;
  }

  .resource-info-title {
    color: #1a365d;
    font-weight: bold;
    font-size: 1.1rem;
    margin-bottom: 2px;
  }

  .resource-info-meta {
    color: #64748b;
    font-size: 13px;
  }

  .resource-btn {
    display: inline-block;
    background-color: #1a365d;
    color: #ffffff !important;
    text-decoration: none !important;
    padding: 8px 16px;
    border-radius: 4px;
    font-size: 14px;
    font-weight: bold;
    transition: background-color 0.2s ease;
  }

  .resource-btn:hover {
    background-color: #2c5282;
  }

  /* Typographical Error Section Styling */
  .typo-section {
    margin-top: 30px;
    padding: 20px;
    background-color: #fef2f2;
    border: 1px dashed #f87171;
    border-radius: 6px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 15px;
  }

  .typo-text {
    color: #991b1b;
    font-size: 14px;
    margin: 0;
    line-height: 1.5;
  }

  .typo-btn {
    display: inline-block;
    background-color: #dc2626;
    color: #ffffff !important;
    text-decoration: none !important;
    padding: 8px 16px;
    border-radius: 4px;
    font-size: 14px;
    font-weight: bold;
    white-space: nowrap;
    transition: background-color 0.2s ease;
  }

  .typo-btn:hover {
    background-color: #b91c1c;
  }
</style>

<!-- Resources Section Container -->
<div class="resources-container">
  <ul class="resources-list">
    <!-- MetaOptics Software Link -->
    <li class="resource-item">
      <div>
        <div class="resource-info-title">MetaOptics</div>
        <div class="resource-info-meta">Windows software</div>
      </div>
      <a href="https://drive.google.com/drive/folders/13JNNMIpgqMMrghrcYjTmmgdcdY4fLALg?usp=sharing" class="resource-btn" target="_blank" rel="noopener noreferrer">Download</a>
    </li>

    <!-- YouTube Playlist Link -->
    <li class="resource-item">
      <div>
        <div class="resource-info-title">Optical Engineering</div>
        <div class="resource-info-meta">YouTube Playlist</div>
      </div>
      <a href="https://youtube.com/playlist?list=PLyqSpQzTE6M9KuQnanecDqCiJUCnCgSQf&si=VSqKrCppMJXX4IwX" class="resource-btn" target="_blank" rel="noopener noreferrer">Watch Playlist</a>
    </li>

    <!-- CNNP Reference Link -->
    <li class="resource-item">
      <div>
        <div class="resource-info-title">Centre for NEMS and Nanophotonics (CNNP)</div>
        <div class="resource-info-meta">Research Facility Website</div>
      </div>
      <a href="https://www.ee.iitm.ac.in/cnnp/" class="resource-btn" target="_blank" rel="noopener noreferrer">Visit Website</a>
    </li>
  </ul>

  <!-- Typographical Error Reporting Block -->
  <div class="typo-section">
    <p class="typo-text">
      Corrections to typos in the book: “Introduction to Ray, Wave, and Beam Optics with Applications,” IOP Publ., November 2024. (ISBN 0750354984, 978075035498)
    </p>
    <a href="https://docs.google.com/document/d/14KOftcBTeISPT5WHueYEvmjChvsAqKXqi4Z-OINyoco/edit?tab=t.0" class="typo-btn" target="_blank" rel="noopener noreferrer">corrections</a>
  </div>
</div>
