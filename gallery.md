---
layout: single
title: "Lab Gallery"
---

<!-- Tailwind CSS for utility styling -->
<script src="https://cdn.tailwindcss.com"></script>
<!-- Font Awesome 6 Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>
  /* Base Brand Typography & Colors */
  body, .gallery-root {
    font-family: 'Calibri', 'Segoe UI', -apple-system, BlinkMacSystemFont, Roboto, sans-serif;
    background-color: #ffffff;
    color: #334155;
  }

  /* Custom Scrollbar Styling */
  ::-webkit-scrollbar {
    width: 8px;
  }
  ::-webkit-scrollbar-track {
    background: #f1f5f9;
  }
  ::-webkit-scrollbar-thumb {
    background: #94a3b8;
    border-radius: 4px;
  }
  ::-webkit-scrollbar-thumb:hover {
    background: #1a365d;
  }

  /* Card Hover Effects */
  .gallery-card {
    transition: transform 0.3s cubic-bezier(0.16, 1, 0.3, 1), box-shadow 0.3s cubic-bezier(0.16, 1, 0.3, 1);
  }
  
  .gallery-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(26, 54, 147, 0.12);
  }

  .gallery-card:hover .card-overlay {
    opacity: 1;
  }

  .gallery-card:hover .card-img {
    transform: scale(1.06);
  }

  .card-img {
    transition: transform 0.5s ease;
  }

  /* Accent Bar */
  .accent-bar {
    width: 60px;
    height: 3px;
    background-color: #38bdf8; /* Cyan accent */
    border-radius: 2px;
  }

  /* Active Filter Tab */
  .filter-tab {
    transition: all 0.25s ease;
  }
  .filter-tab.active {
    background-color: #1a365d; /* Dark brand blue */
    color: #ffffff;
    border-color: #1a365d;
    box-shadow: 0 4px 12px rgba(26, 54, 147, 0.2);
  }

  /* Modal Zoom Keyframes */
  @keyframes modalFadeIn {
    from {
      opacity: 0;
      transform: scale(0.96);
    }
    to {
      opacity: 1;
      transform: scale(1);
    }
  }

  .animate-modal {
    animation: modalFadeIn 0.25s ease-out forwards;
  }
</style>

<div class="gallery-root min-h-screen flex flex-col justify-between antialiased">

  <!-- Header / Hero Section (Clean Layout Starting Directly with Title & Subtitle) -->
  <section class="bg-gradient-to-b from-[#f8fafc] to-white py-10 md:py-12 border-b border-[#e2e8f0]">
    <div class="max-w-6xl mx-auto px-4 text-center">
      
      <!-- Main Title -->
      <h1 class="text-3xl sm:text-4xl md:text-5xl font-bold text-[#1a365d] tracking-tight">
        Visual Archives & Lab Gallery
      </h1>

      <!-- Divider Bar -->
      <div class="accent-bar mx-auto my-4"></div>

      <!-- Subtitle Description -->
      <p class="text-slate-600 text-base md:text-lg max-w-3xl mx-auto leading-relaxed">
        High-resolution visual record of experimental setups, research milestones, optics facilities, and academic events at the <strong>Applied Optics Group</strong>, IIT Madras.
      </p>

      <!-- Quick Metrics & Navigation Bar -->
      <div class="mt-8 flex flex-wrap items-center justify-center gap-3 text-xs md:text-sm font-medium text-slate-600">
        <span class="bg-[#f8fafc] border border-[#e2e8f0] px-4 py-1.5 rounded-full flex items-center gap-2 shadow-sm">
          <i class="fa-solid fa-camera text-[#38bdf8]"></i> <span id="stat-total-count">0</span> Photos
        </span>
        <span class="bg-[#f8fafc] border border-[#e2e8f0] px-4 py-1.5 rounded-full flex items-center gap-2 shadow-sm">
          <i class="fa-solid fa-layer-group text-[#38bdf8]"></i> 4 Categories
        </span>
        <a href="{{ '/' | relative_url }}" class="inline-flex items-center gap-2 bg-[#1a365d] hover:bg-[#38bdf8] text-white hover:text-[#1a365d] px-5 py-1.5 rounded-full font-bold transition-all duration-300 shadow-sm">
          <i class="fa-solid fa-house"></i> Return to Home Page
        </a>
      </div>

    </div>
  </section>

  <!-- Controls & Gallery Area -->
  <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 flex-grow w-full">
    
    <!-- Filter and Search Bar Container -->
    <div class="flex flex-col lg:flex-row lg:items-center justify-between gap-4 mb-8 bg-[#f8fafc] p-4 rounded-2xl border border-[#e2e8f0]">
      
      <!-- Category Filter Tabs -->
      <div class="flex flex-wrap items-center gap-2" id="category-tabs">
        <button onclick="filterCategory('All')" class="filter-tab active px-4 py-2 rounded-xl text-xs sm:text-sm font-bold border border-slate-300 text-slate-700 hover:bg-slate-100">
          All Archives
        </button>
        <button onclick="filterCategory('Lab & Equipment')" class="filter-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-bold border border-slate-300 text-slate-700 hover:bg-slate-100">
          Lab & Equipment
        </button>
        <button onclick="filterCategory('Research Highlights')" class="filter-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-bold border border-slate-300 text-slate-700 hover:bg-slate-100">
          Research Highlights
        </button>
        <button onclick="filterCategory('Conferences & Events')" class="filter-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-bold border border-slate-300 text-slate-700 hover:bg-slate-100">
          Conferences
        </button>
        <button onclick="filterCategory('Group Photos')" class="filter-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-bold border border-slate-300 text-slate-700 hover:bg-slate-100">
          Group Photos
        </button>
      </div>

      <!-- Real-Time Search Box -->
      <div class="relative min-w-[240px] lg:w-80">
        <div class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400">
          <i class="fa-solid fa-magnifying-glass text-sm"></i>
        </div>
        <input 
          type="text" 
          id="search-input" 
          oninput="handleSearch()"
          placeholder="Search by keywords, tags, or topic..." 
          class="w-full pl-10 pr-4 py-2 bg-white border border-slate-300 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-[#38bdf8] focus:border-[#1a365d] transition-all"
        >
      </div>

    </div>

    <!-- Active Item Count Summary -->
    <div class="flex items-center justify-between mb-6 px-1">
      <div class="text-xs sm:text-sm text-slate-600 font-medium" id="results-count">
        Loading photo archives...
      </div>
      <div class="text-xs text-slate-400 italic">
        Click any image to open full resolution viewer
      </div>
    </div>

    <!-- Gallery Grid -->
    <div id="gallery-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6">
      <!-- Dynamic Photo Cards injected via JS -->
    </div>

    <!-- Empty Search Results State -->
    <div id="empty-state" class="hidden text-center py-16 bg-[#f8fafc] rounded-2xl border border-dashed border-slate-300 my-8">
      <div class="w-16 h-16 mx-auto mb-4 rounded-full bg-slate-100 flex items-center justify-center text-slate-400 text-2xl">
        <i class="fa-solid fa-folder-open"></i>
      </div>
      <h3 class="text-lg font-bold text-[#1a365d]">No Matching Photos Found</h3>
      <p class="text-slate-500 text-sm mt-1 max-w-md mx-auto">Try typing a different search term or select another category filter above.</p>
      <button onclick="resetFilters()" class="mt-4 px-4 py-2 bg-[#1a365d] text-white rounded-lg text-xs font-bold hover:bg-[#38bdf8] hover:text-[#1a365d] transition-colors">
        Reset All Filters
      </button>
    </div>

  </main>

  <!-- Lightbox Modal -->
  <div id="lightbox-modal" class="fixed inset-0 z-50 hidden bg-slate-950/90 backdrop-blur-md flex items-center justify-center p-3 sm:p-6 transition-opacity duration-300">
    
    <!-- Modal Container -->
    <div class="relative max-w-5xl w-full bg-[#f8fafc] rounded-2xl overflow-hidden shadow-2xl border border-slate-700 flex flex-col max-h-[92vh] animate-modal">
      
      <!-- Top Modal Bar -->
      <div class="bg-[#1a365d] text-white px-5 py-3.5 flex items-center justify-between border-b border-slate-700">
        <div class="flex items-center space-x-3 truncate pr-4">
          <span id="modal-category-badge" class="bg-[#38bdf8] text-[#1a365d] text-xs font-extrabold px-2.5 py-1 rounded-md uppercase tracking-wider">
            Category
          </span>
          <h3 id="modal-title" class="font-bold text-base sm:text-lg truncate">
            Photo Title
          </h3>
        </div>

        <div class="flex items-center space-x-2">
          <span id="modal-counter" class="text-xs text-slate-300 font-mono hidden sm:inline-block mr-2">
            1 / 12
          </span>
          <button onclick="closeLightbox()" class="w-9 h-9 rounded-full bg-slate-800 hover:bg-red-500 text-white flex items-center justify-center transition-colors">
            <i class="fa-solid fa-xmark text-lg"></i>
          </button>
        </div>
      </div>

      <!-- Center Modal Body (Image & Arrows) -->
      <div class="relative bg-black flex-grow flex items-center justify-center min-h-[300px] max-h-[65vh] overflow-hidden group">
        
        <!-- Main Image -->
        <img id="modal-image" src="" alt="" class="max-h-[65vh] w-auto max-w-full object-contain mx-auto select-none">

        <!-- Nav Previous -->
        <button onclick="prevImage()" class="absolute left-3 top-1/2 -translate-y-1/2 w-11 h-11 rounded-full bg-slate-900/70 hover:bg-[#38bdf8] text-white hover:text-[#1a365d] flex items-center justify-center transition-all shadow-lg backdrop-blur-sm">
          <i class="fa-solid fa-chevron-left text-lg"></i>
        </button>

        <!-- Nav Next -->
        <button onclick="nextImage()" class="absolute right-3 top-1/2 -translate-y-1/2 w-11 h-11 rounded-full bg-slate-900/70 hover:bg-[#38bdf8] text-white hover:text-[#1a365d] flex items-center justify-center transition-all shadow-lg backdrop-blur-sm">
          <i class="fa-solid fa-chevron-right text-lg"></i>
        </button>
      </div>

      <!-- Bottom Modal Description -->
      <div class="p-5 bg-white border-t border-slate-200">
        <p id="modal-caption" class="text-slate-700 text-sm sm:text-base leading-relaxed mb-3">
          Photo caption description goes here...
        </p>
        
        <div class="flex flex-wrap items-center justify-between gap-2 pt-2 border-t border-slate-100 text-xs text-slate-500">
          <div class="flex flex-wrap items-center gap-4">
            <span><i class="fa-regular fa-calendar text-[#38bdf8] mr-1.5"></i> <span id="modal-date">Date</span></span>
            <span><i class="fa-solid fa-tags text-[#38bdf8] mr-1.5"></i> <span id="modal-tags">Tags</span></span>
          </div>
          <span class="text-slate-400 hidden sm:inline">Use Left/Right Arrow Keys (&#8592; &#8594;) to switch photos</span>
        </div>
      </div>

    </div>
  </div>

</div>

<!-- Interactive Gallery Logic Script -->
<script>
  /* ==========================================================================
     HOW TO ADD OR MODIFY PHOTOS IN THIS GALLERY:
     --------------------------------------------------------------------------
     Add a new JS object inside the `galleryData` array with the following:
     {
       id: 13,
       title: "Your Photo Title",
       category: "Lab & Equipment", // Options: 'Lab & Equipment', 'Research Highlights', 'Conferences & Events', 'Group Photos'
       date: "March 2026",
       src: "/assets/images/gallery/photo1.jpg", // Path to your photo file or external image URL
       caption: "Detailed description of the experiment or photo.",
       tags: ["tag1", "tag2", "tag3"]
     }
     ========================================================================== */

  const galleryData = [
    {
      id: 1,
      title: "Optical Tweezers & Trapping Setup",
      category: "Lab & Equipment",
      date: "February 2025",
      src: "https://images.unsplash.com/photo-1507668077129-56e32842fceb?auto=format&fit=crop&w=800&q=80",
      caption: "High-precision optical tweezers workstation with 1064nm CW Nd:YAG laser and spatial light modulator for particle trapping.",
      tags: ["optical tweezers", "laser trapping", "1064nm", "slm", "microscope"]
    },
    {
      id: 2,
      title: "Digital Holographic Interferometry Testbed",
      category: "Research Highlights",
      date: "January 2025",
      src: "https://images.unsplash.com/photo-1509228468518-180dd4864904?auto=format&fit=crop&w=800&q=80",
      caption: "Mach-Zehnder digital holographic setup configured for label-free 3D quantitative phase tomography.",
      tags: ["holography", "interferometry", "mach zehnder", "3d imaging", "phase"]
    },
    {
      id: 3,
      title: "Applied Optics Group Annual Photo",
      category: "Group Photos",
      date: "January 2025",
      src: "https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&w=800&q=80",
      caption: "Group scholars, faculty, and research personnel gathered outside the Electrical Engineering Department building.",
      tags: ["group photo", "team", "iit madras", "research scholars"]
    },
    {
      id: 4,
      title: "SPIE Optics & Photonics Presentation",
      category: "Conferences & Events",
      date: "August 2024",
      src: "https://images.unsplash.com/photo-1475721027785-f74eccf877e2?auto=format&fit=crop&w=800&q=80",
      caption: "Research scholars presenting poster sessions on quantitative phase recovery at SPIE Optics & Photonics.",
      tags: ["spie", "conference", "presentation", "poster session"]
    },
    {
      id: 5,
      title: "Femtosecond Laser Micro-Machining Station",
      category: "Lab & Equipment",
      date: "November 2024",
      src: "https://images.unsplash.com/photo-1581093458791-9f3c3900df4b?auto=format&fit=crop&w=800&q=80",
      caption: "Ultrafast femtosecond laser system used for waveguide writing and precision surface micro-structuring.",
      tags: ["femtosecond", "ultrafast laser", "micro machining", "waveguide"]
    },
    {
      id: 6,
      title: "Live Cell Quantitative Phase Bio-Imaging",
      category: "Research Highlights",
      date: "December 2024",
      src: "https://images.unsplash.com/photo-1576086213369-97a306d36557?auto=format&fit=crop&w=800&q=80",
      caption: "Label-free live cell dynamics profiling with off-axis digital holographic microscopy.",
      tags: ["bio imaging", "live cell", "microscopy", "quantitative phase"]
    },
    {
      id: 7,
      title: "Optica Student Chapter Workshop",
      category: "Conferences & Events",
      date: "October 2024",
      src: "https://images.unsplash.com/photo-1531482615713-2afd69097998?auto=format&fit=crop&w=800&q=80",
      caption: "Hands-on optical diffraction and microscopy workshop organized by student chapter members.",
      tags: ["workshop", "student chapter", "optica", "outreach"]
    },
    {
      id: 8,
      title: "Photonic Crystal Fiber Testbed",
      category: "Lab & Equipment",
      date: "September 2024",
      src: "https://images.unsplash.com/photo-1518770660439-4636190af475?auto=format&fit=crop&w=800&q=80",
      caption: "Supercontinuum generation setup utilizing PCF pumped by pulsed nanosecond laser source.",
      tags: ["fiber optics", "supercontinuum", "photonic crystal fiber"]
    },
    {
      id: 9,
      title: "Adaptive Optics Aberration Correction",
      category: "Research Highlights",
      date: "July 2024",
      src: "https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?auto=format&fit=crop&w=800&q=80",
      caption: "Closed-loop deformable mirror testbed designed for correcting optical aberrations in deep tissue imaging.",
      tags: ["adaptive optics", "wavefront sensor", "deformable mirror"]
    },
    {
      id: 10,
      title: "Applied Optics Group Retreat",
      category: "Group Photos",
      date: "May 2024",
      src: "https://images.unsplash.com/photo-1511578314322-379afb476865?auto=format&fit=crop&w=800&q=80",
      caption: "Group members participating in the annual laboratory retreat and team activity near Mahabalipuram.",
      tags: ["retreat", "outing", "team building"]
    },
    {
      id: 11,
      title: "Fiber Bragg Grating Interrogator System",
      category: "Lab & Equipment",
      date: "April 2024",
      src: "https://images.unsplash.com/photo-1532094349884-543bc11b234d?auto=format&fit=crop&w=800&q=80",
      caption: "Optical sensing interrogation platform for strain and temperature sensing using multiplexed FBGs.",
      tags: ["fbg", "fiber sensing", "interrogator"]
    },
    {
      id: 12,
      title: "National Laser Symposium Paper Award",
      category: "Conferences & Events",
      date: "January 2024",
      src: "https://images.unsplash.com/photo-1517077304055-6e89abbf09b0?auto=format&fit=crop&w=800&q=80",
      caption: "Recognition awarded at NLS for paper on quantitative spatial phase filtering techniques.",
      tags: ["award", "nls", "symposium", "conference"]
    }
  ];

  /* State Variables */
  let currentCategory = 'All';
  let currentSearchTerm = '';
  let filteredItems = [...galleryData];
  let activeModalIndex = 0;

  /* On DOM Ready */
  document.addEventListener('DOMContentLoaded', () => {
    document.getElementById('stat-total-count').textContent = galleryData.length;
    renderGallery();

    /* Keyboard Navigation for Lightbox */
    document.addEventListener('keydown', (e) => {
      const modal = document.getElementById('lightbox-modal');
      if (!modal.classList.contains('hidden')) {
        if (e.key === 'Escape') closeLightbox();
        if (e.key === 'ArrowLeft') prevImage();
        if (e.key === 'ArrowRight') nextImage();
      }
    });
  });

  /* Main Gallery Render Function */
  function renderGallery() {
    const grid = document.getElementById('gallery-grid');
    const emptyState = document.getElementById('empty-state');
    const resultsCounter = document.getElementById('results-count');

    // Filter Items
    filteredItems = galleryData.filter(item => {
      const matchesCategory = (currentCategory === 'All') || (item.category === currentCategory);
      
      const term = currentSearchTerm.toLowerCase();
      const matchesSearch = !term || 
        item.title.toLowerCase().includes(term) || 
        item.caption.toLowerCase().includes(term) ||
        item.category.toLowerCase().includes(term) ||
        item.tags.some(tag => tag.toLowerCase().includes(term));

      return matchesCategory && matchesSearch;
    });

    resultsCounter.textContent = `Showing ${filteredItems.length} of ${galleryData.length} photo entries`;

    if (filteredItems.length === 0) {
      grid.innerHTML = '';
      emptyState.classList.remove('hidden');
      return;
    }

    emptyState.classList.add('hidden');

    grid.innerHTML = filteredItems.map((item, index) => {
      return `
        <div 
          onclick="openLightbox(${index})"
          class="gallery-card bg-[#f8fafc] border border-[#e2e8f0] rounded-2xl overflow-hidden cursor-pointer flex flex-col group"
        >
          <!-- Thumbnail -->
          <div class="relative h-52 bg-slate-900 overflow-hidden">
            <img 
              src="${item.src}" 
              alt="${item.title}" 
              class="card-img w-full h-full object-cover"
              loading="lazy"
              onerror="this.onerror=null; this.src='https://placehold.co/800x600/1a365d/38bdf8?text=Applied+Optics+Group';"
            />
            
            <!-- Hover Magnifier Icon -->
            <div class="card-overlay absolute inset-0 bg-[#1a365d]/70 opacity-0 flex items-center justify-center transition-opacity duration-300">
              <div class="w-11 h-11 rounded-full bg-[#38bdf8] text-[#1a365d] flex items-center justify-center text-lg shadow-lg transform translate-y-2 group-hover:translate-y-0 transition-transform duration-300">
                <i class="fa-solid fa-magnifying-glass-plus"></i>
              </div>
            </div>

            <!-- Top Category Tag -->
            <span class="absolute top-3 left-3 bg-[#1a365d]/90 backdrop-blur-sm text-[#38bdf8] text-[10px] font-extrabold uppercase tracking-wider px-2.5 py-1 rounded-md border border-[#38bdf8]/30">
              ${item.category}
            </span>
          </div>

          <!-- Card Content -->
          <div class="p-4 flex-grow flex flex-col justify-between">
            <div>
              <h3 class="font-bold text-[#1a365d] text-base line-clamp-1 group-hover:text-[#38bdf8] transition-colors">
                ${item.title}
              </h3>
              <p class="text-xs text-slate-500 mt-1 line-clamp-2 leading-relaxed">
                ${item.caption}
              </p>
            </div>

            <!-- Tags & Date Footer -->
            <div class="mt-4 pt-3 border-t border-slate-200 flex items-center justify-between text-xs text-slate-400 font-medium">
              <span><i class="fa-regular fa-calendar text-[#38bdf8] mr-1"></i> ${item.date}</span>
              <span class="text-[#1a365d] font-semibold flex items-center gap-1 group-hover:translate-x-1 transition-transform">
                Expand <i class="fa-solid fa-arrow-right text-[10px]"></i>
              </span>
            </div>
          </div>
        </div>
      `;
    }).join('');
  }

  /* Filter Switcher */
  function filterCategory(category) {
    currentCategory = category;

    const buttons = document.querySelectorAll('#category-tabs button');
    buttons.forEach(btn => {
      if (btn.textContent.trim().startsWith(category) || (category === 'All' && btn.textContent.trim().startsWith('All'))) {
        btn.classList.add('active');
      } else {
        btn.classList.remove('active');
      }
    });

    renderGallery();
  }

  /* Search Trigger */
  function handleSearch() {
    currentSearchTerm = document.getElementById('search-input').value;
    renderGallery();
  }

  /* Reset Filter Controls */
  function resetFilters() {
    document.getElementById('search-input').value = '';
    currentSearchTerm = '';
    filterCategory('All');
  }

  /* Lightbox Controls */
  function openLightbox(index) {
    activeModalIndex = index;
    updateLightboxContent();
    const modal = document.getElementById('lightbox-modal');
    modal.classList.remove('hidden');
    document.body.style.overflow = 'hidden';
  }

  function closeLightbox() {
    const modal = document.getElementById('lightbox-modal');
    modal.classList.add('hidden');
    document.body.style.overflow = 'auto';
  }

  function updateLightboxContent() {
    const item = filteredItems[activeModalIndex];
    if (!item) return;

    document.getElementById('modal-title').textContent = item.title;
    document.getElementById('modal-category-badge').textContent = item.category;
    document.getElementById('modal-image').src = item.src;
    document.getElementById('modal-caption').textContent = item.caption;
    document.getElementById('modal-date').textContent = item.date;
    document.getElementById('modal-tags').textContent = item.tags.join(', ');
    document.getElementById('modal-counter').textContent = `${activeModalIndex + 1} / ${filteredItems.length}`;
  }

  function nextImage() {
    if (filteredItems.length === 0) return;
    activeModalIndex = (activeModalIndex + 1) % filteredItems.length;
    updateLightboxContent();
  }

  function prevImage() {
    if (filteredItems.length === 0) return;
    activeModalIndex = (activeModalIndex - 1 + filteredItems.length) % filteredItems.length;
    updateLightboxContent();
  }
</script>
