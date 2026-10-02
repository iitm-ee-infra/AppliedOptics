---
layout: single
title: "Lab Gallery"
# --- GALLERY ASSETS CONFIGURATION ---
# Place your image files in your site's asset folder (e.g., assets/images/gallery/)
# You can easily edit titles, categories, and captions below:
gallery_images:
  - url: "/assets/img/group.png"
    title: "Convocation 2026"
    category: "team"
    caption: "Convocation 2026"

  - url: "/assets/img/FOP_26.jpg"
    title: "FRONTIERS IN OPTICS AND PHOTONICS (FOP) 2026"
    category: "team"
    caption: "FRONTIERS IN OPTICS AND PHOTONICS (FOP) 2026, September 25 - 28, 2026 JOINTLY ORGANIZED BY INDIAN INSTITUTE OF TECHNOLOGY DELHI (IITD) AND CSIR-NATIONAL PHYSICAL LABORATORY (CSIR-NPL)"


---

<div class="gallery-page-container">

  <!-- Header Banner -->
  <div class="gallery-header-card">
    <div class="icon-wrapper">
      <i class="fa fa-picture-o mechanical-gear"></i>
      <i class="fa fa-camera sub-tool-icon"></i>
    </div>

    <h1 class="maintenance-title">Applied Optics Group Gallery</h1>
    <div class="accent-bar"></div>

   

    <!-- Category Filter Bar -->
    <div class="filter-wrapper">
      <button class="filter-btn active" data-filter="all">
        <i class="fa fa-th-large"></i> All Photos
      </button>
      <button class="filter-btn" data-filter="research">
        <i class="fa fa-flask"></i> Research
      </button>
      <button class="filter-btn" data-filter="equipment">
        <i class="fa fa-cogs"></i> Equipment
      </button>
      <button class="filter-btn" data-filter="team">
        <i class="fa fa-users"></i> Group Photos
      </button>
    </div>
  </div>

  <!-- Gallery Image Grid -->
  <div class="gallery-grid" id="galleryGrid">
    {% for item in page.gallery_images %}
    <div class="gallery-item-card" data-category="{{ item.category }}">
      <div class="image-wrapper" onclick="openLightbox('{{ item.url | relative_url }}', '{{ item.title | escape }}', '{{ item.caption | escape }}')">
        <img src="{{ item.url | relative_url }}" alt="{{ item.title }}" loading="lazy" onerror="this.onerror=null; this.src='https://via.placeholder.com/600x400/1a365d/ffffff?text=Image+Placeholder';">
        <div class="image-overlay">
          <i class="fa fa-search-plus overlay-icon"></i>
          <span class="view-text">Click to Expand</span>
        </div>
      </div>
      <div class="card-details">
        <span class="category-badge">{{ item.category | capitalize }}</span>
        <h3 class="card-title">{{ item.title }}</h3>
        <p class="card-caption">{{ item.caption }}</p>
      </div>
    </div>
    {% endfor %}
  </div>

  <!-- Return Home Button -->
  <div class="return-home-container">
    <a href="{{ '/' | relative_url }}" class="return-home-btn">
      <i class="fa fa-home" style="margin-right: 8px;"></i>Return to Home Page
    </a>
  </div>

</div>

<!-- Lightbox Modal Viewer -->
<div id="lightboxModal" class="lightbox-modal" onclick="closeLightboxOnBg(event)">
  <span class="lightbox-close" onclick="closeLightbox()">&times;</span>
  <div class="lightbox-content-wrapper">
    <img id="lightboxImg" class="lightbox-image" src="" alt="Enlarged View">
    <div class="lightbox-caption-box">
      <h3 id="lightboxTitle"></h3>
      <p id="lightboxCaption"></p>
    </div>
  </div>
</div>

<!-- Embedded Clean CSS Layout -->
<style>
  .gallery-page-container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 20px;
    background-color: #ffffff;
    font-family: 'Calibri', sans-serif;
  }

  .gallery-header-card {
    text-align: center;
    background: #f8fafc;
    border: 1px solid #e2e8f0;
    border-radius: 12px;
    padding: 35px 25px 25px 25px;
    margin-bottom: 35px;
    box-shadow: 0 10px 25px rgba(26, 54, 147, 0.04);
  }

  .icon-wrapper {
    position: relative;
    display: inline-block;
    margin-bottom: 15px;
  }

  .mechanical-gear {
    font-size: 3.8rem;
    color: #1a365d;
  }

  .sub-tool-icon {
    position: absolute;
    bottom: -4px;
    right: -8px;
    font-size: 1.5rem;
    color: #38bdf8;
    background: #f8fafc;
    padding: 3px;
    border-radius: 50%;
  }

  .maintenance-title {
    color: #1a365d;
    font-family: 'Calibri', sans-serif;
    font-weight: bold;
    font-size: 2.2rem;
    margin-bottom: 0;
    margin-top: 5px;
  }

  .accent-bar {
    width: 60px;
    height: 3px;
    background-color: #38bdf8;
    margin: 15px auto 18px auto;
    border-radius: 2px;
  }

  .maintenance-message {
    color: #334155;
    font-size: 16px;
    line-height: 1.6;
    max-width: 650px;
    margin: 0 auto 25px auto;
  }

  /* Filter Navigation Tabs */
  .filter-wrapper {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 15px;
  }

  .filter-btn {
    background-color: #ffffff;
    color: #1a365d;
    border: 1px solid #cbd5e1;
    padding: 8px 18px;
    border-radius: 20px;
    font-size: 14px;
    font-weight: bold;
    cursor: pointer;
    transition: all 0.25s ease;
  }

  .filter-btn i {
    margin-right: 5px;
    color: #38bdf8;
  }

  .filter-btn:hover {
    background-color: #38bdf8;
    color: #1a365d;
    border-color: #38bdf8;
  }

  .filter-btn:hover i {
    color: #1a365d;
  }

  .filter-btn.active {
    background-color: #1a365d;
    color: #ffffff;
    border-color: #1a365d;
  }

  .filter-btn.active i {
    color: #38bdf8;
  }

  /* Gallery Grid Layout */
  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 25px;
    margin-bottom: 40px;
  }

  .gallery-item-card {
    background: #f8fafc;
    border: 1px solid #e2e8f0;
    border-radius: 12px;
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
  }

  .gallery-item-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 25px rgba(26, 54, 147, 0.12);
  }

  .image-wrapper {
    position: relative;
    width: 100%;
    height: 220px;
    overflow: hidden;
    cursor: pointer;
    background-color: #e2e8f0;
  }

  .image-wrapper img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.4s ease;
  }

  .gallery-item-card:hover .image-wrapper img {
    transform: scale(1.06);
  }

  .image-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(26, 54, 147, 0.75);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: opacity 0.3s ease;
    color: #ffffff;
  }

  .image-wrapper:hover .image-overlay {
    opacity: 1;
  }

  .overlay-icon {
    font-size: 2rem;
    color: #38bdf8;
    margin-bottom: 6px;
  }

  .view-text {
    font-size: 13px;
    font-weight: bold;
    letter-spacing: 0.5px;
    text-transform: uppercase;
  }

  .card-details {
    padding: 18px 20px;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }

  .category-badge {
    align-self: flex-start;
    background-color: rgba(56, 189, 248, 0.15);
    color: #1a365d;
    font-size: 11px;
    font-weight: bold;
    padding: 3px 10px;
    border-radius: 12px;
    margin-bottom: 8px;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .card-title {
    color: #1a365d;
    font-size: 1.15rem;
    font-weight: bold;
    margin: 0 0 8px 0;
  }

  .card-caption {
    color: #64748b;
    font-size: 13.5px;
    line-height: 1.5;
    margin: 0;
  }

  .return-home-container {
    text-align: center;
    margin-top: 20px;
    margin-bottom: 20px;
  }

  .return-home-btn {
    display: inline-block;
    background-color: #1a365d;
    color: #ffffff !important;
    font-family: 'Calibri', sans-serif;
    font-weight: bold;
    font-size: 15px;
    padding: 10px 24px;
    border-radius: 30px;
    text-decoration: none !important;
    transition: all 0.3s ease;
    box-shadow: 0 4px 10px rgba(26, 54, 147, 0.15);
  }

  .return-home-btn:hover {
    background-color: #38bdf8;
    color: #1a365d !important;
    transform: translateY(-2px);
  }

  /* Lightbox Modal */
  .lightbox-modal {
    display: none;
    position: fixed;
    z-index: 9999;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(15, 23, 42, 0.88);
    backdrop-filter: blur(4px);
    justify-content: center;
    align-items: center;
    padding: 20px;
    box-sizing: border-box;
  }

  .lightbox-content-wrapper {
    max-width: 850px;
    width: 100%;
    background: #ffffff;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(0,0,0,0.4);
    animation: zoomIn 0.25s ease-out;
  }

  @keyframes zoomIn {
    from { transform: scale(0.9); opacity: 0; }
    to { transform: scale(1); opacity: 1; }
  }

  .lightbox-image {
    width: 100%;
    max-height: 70vh;
    object-fit: contain;
    background-color: #0f172a;
    display: block;
  }

  .lightbox-caption-box {
    padding: 20px 25px;
    background-color: #f8fafc;
    border-top: 1px solid #e2e8f0;
  }

  .lightbox-caption-box h3 {
    color: #1a365d;
    margin: 0 0 6px 0;
    font-size: 1.3rem;
  }

  .lightbox-caption-box p {
    color: #334155;
    margin: 0;
    font-size: 14.5px;
    line-height: 1.5;
  }

  .lightbox-close {
    position: absolute;
    top: 20px;
    right: 30px;
    color: #ffffff;
    font-size: 38px;
    font-weight: bold;
    cursor: pointer;
    transition: color 0.2s ease;
  }

  .lightbox-close:hover {
    color: #38bdf8;
  }
</style>

<!-- Embedded Interactive JavaScript -->
<script>
  document.addEventListener('DOMContentLoaded', function () {
    // Filter Category Logic
    const filterBtns = document.querySelectorAll('.filter-btn');
    const galleryItems = document.querySelectorAll('.gallery-item-card');

    filterBtns.forEach(btn => {
      btn.addEventListener('click', function () {
        filterBtns.forEach(b => b.classList.remove('active'));
        this.classList.add('active');

        const filterValue = this.getAttribute('data-filter');

        galleryItems.forEach(item => {
          if (filterValue === 'all' || item.getAttribute('data-category') === filterValue) {
            item.style.display = 'flex';
          } else {
            item.style.display = 'none';
          }
        });
      });
    });
  });

  // Lightbox Modal Functions
  function openLightbox(imgSrc, title, caption) {
    const modal = document.getElementById('lightboxModal');
    document.getElementById('lightboxImg').src = imgSrc;
    document.getElementById('lightboxTitle').textContent = title;
    document.getElementById('lightboxCaption').textContent = caption;
    modal.style.display = 'flex';
  }

  function closeLightbox() {
    document.getElementById('lightboxModal').style.display = 'none';
  }

  function closeLightboxOnBg(e) {
    if (e.target.id === 'lightboxModal') {
      closeLightbox();
    }
  }

  // Keyboard escape key to close lightbox
  document.addEventListener('keydown', function (e) {
    if (e.key === 'Escape') {
      closeLightbox();
    }
  });
</script>
