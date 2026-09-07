---
layout: single
title: "Publications & Research"
---

<!-- Plain Text Title Block (Centered) -->
<div class="container" style="padding-top: 20px; padding-bottom: 20px; text-align: center;">
  <h1 style="color: #1a365d; font-family: 'Calibri', sans-serif; font-weight: bold; font-size: 3rem; margin-bottom: 0;">
    Research Publications and Talks
  </h1>
  <hr style="border-top: 2px solid #1a365d; margin: 15px auto 0 auto; width: 50%;">
</div>

<!-- CSS Styling for Academic Collapsible Sections & Publication Layout -->
<style>
  .pub-container {
    max-width: 900px;
    margin: 0 auto;
    padding: 20px 0;
    font-family: 'Calibri', sans-serif;
  }

  /* Collapsible Section Styling */
  .collapsible-section {
    background-color: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 8px;
    margin-bottom: 16px;
    box-shadow: 0 2px 6px rgba(26, 54, 93, 0.05);
    overflow: hidden;
    transition: all 0.2s ease-in-out;
  }

  .collapsible-section[open] {
    border-color: #1a365d;
    box-shadow: 0 4px 12px rgba(26, 54, 93, 0.1);
  }

  .collapsible-header {
    font-size: 1.35rem;
    font-weight: bold;
    color: #1a365d;
    background-color: #f8fafc;
    padding: 16px 20px;
    cursor: pointer;
    user-select: none;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid transparent;
  }

  .collapsible-section[open] > .collapsible-header {
    background-color: #1a365d;
    color: #ffffff;
    border-bottom: 1px solid #1a365d;
  }

  .collapsible-header::-webkit-details-marker {
    display: none;
  }

  .collapsible-header::after {
    content: "►";
    font-size: 0.9rem;
    transition: transform 0.2s ease;
  }

  .collapsible-section[open] > .collapsible-header::after {
    transform: rotate(90deg);
  }

  /* Nested Collapsible for Conferences */
  .nested-collapsible {
    margin: 15px 20px;
    border: 1px solid #cbd5e1;
    border-radius: 6px;
  }

  .nested-header {
    font-size: 1.15rem;
    font-weight: bold;
    color: #1a365d;
    background-color: #f1f5f9;
    padding: 12px 16px;
    cursor: pointer;
    user-select: none;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .nested-collapsible[open] > .nested-header {
    background-color: #334155;
    color: #ffffff;
  }

  .nested-header::-webkit-details-marker {
    display: none;
  }

  .nested-header::after {
    content: "►";
    font-size: 0.8rem;
    transition: transform 0.2s ease;
  }

  .nested-collapsible[open] > .nested-header::after {
    transform: rotate(90deg);
  }

  /* Publication Item Styling */
  .pub-content {
    padding: 20px;
  }

  .pub-list {
    list-style: none;
    padding-left: 0;
    margin: 0;
  }

  .pub-item {
    font-size: 16px;
    line-height: 1.6;
    color: #1e293b;
    margin-bottom: 18px;
    padding-bottom: 15px;
    border-bottom: 1px solid #f1f5f9;
  }

  .pub-item:last-child {
    border-bottom: none;
    margin-bottom: 0;
    padding-bottom: 0;
  }

  .pub-item em {
    color: #475569;
    font-style: italic;
  }

  .pub-item a {
    color: #1a365d;
    text-decoration: underline;
  }
</style>

<div class="container">
  <div class="pub-container">

    <!-- 1. BOOKS AND BOOK CHAPTERS -->
    <details class="collapsible-section" open>
      <summary class="collapsible-header">Books and Book Chapters</summary>
      <div class="pub-content">
        <ul class="pub-list">
          <li class="pub-item">
            Shanti Bhattacharya, "Introduction to Ray, Wave, and Beam Optics with Applications," <em>IOP Publ.</em>, November 2024. (ISBN 0750354984, 978075035498)[cite: 3]
          </li>
          <li class="pub-item">
            Shanti Bhattacharya, "Six Myopic Engineers and the ?? System," in <em>Field Guide to Optics Education: A Tribute to John Greivenkamp</em>, Ed. J. Scott Tyo and Eric Pepper, SPIE, 2022. <a href="https://doi.org/10.1117/3.2635872.sup" target="_blank">https://doi.org/10.1117/3.2635872.sup</a>[cite: 3]
          </li>
          <li class="pub-item">
            Shanti Bhattacharya and Anand Vijayakumar, "Design and Fabrication of Diffractive Optical Elements with MATLAB," <em>SPIE Press book</em>, January 2017. <a href="http://spie.org/Publications/Book/2261460?&origin_id=x646" target="_blank">SPIE Book Link</a>[cite: 3]
          </li>
        </ul>
      </div>
    </details>

    <!-- 2. REFEREED JOURNALS -->
    <details class="collapsible-section">
      <summary class="collapsible-header">Refereed Journals</summary>
      <div class="pub-content">
        <ul class="pub-list">
          <li class="pub-item">Susan Thomas, Shanti Bhattacharya, and Francesco Ferranti, "Metasurface integrated optics for fluorescence imaging endoscopy," <em>Opt. Express</em> 34, 19686-19700 (2026).[cite: 3]</li>
          <li class="pub-item">Naveen Kumar P, R. David Koilpillai, Shanti Bhattacharya, "Enhanced A-scan spatial resolution in spectral domain OCT exploiting the Wigner-Ville technique," <em>Opt. and Las. in Engg.</em>, 186, 108736 (2025).[cite: 3]</li>
          <li class="pub-item">C. Taneja, J. G. George, S. Corsetti, P. Wijesinghe, G. D. Bruce, M. F. Zwart, S. Bhattacharya, and K. Dholakia, "Sidelobe suppressed Bessel beams for one-photon light-sheet microscopy," <em>Biomed. Opt. Express</em> 15, 6183-6197 (2024).[cite: 3]</li>
          <li class="pub-item">Jerin Geogy George, Shanti Bhattacharya, "Overcoming challenges in fabrication of beam shaping meta-optics using sensitive mr-EBL resist," <em>J. Optical Microsystems</em> 4(4) 041402 (2024).[cite: 3]</li>
          <li class="pub-item">Susan Thomas, Jerin Geogy George, Francesco Ferranti, Shanti Bhattacharya, "Metaoptics for aberration correction in microendoscopy," <em>Opt. Exp.</em> 32(6), 9686-9698 (2024).[cite: 3]</li>
          <li class="pub-item">Debdutta Basu, Suresh Chejarla, Satyajit Maji, Shanti Bhattacharya, Balaji Srinivasan, "An adaptive optical technique for structured beam generation based on phase retrieval using modified Gerchberg–Saxton algorithm," <em>Opt. & Laser Tech.</em> 170, 110244 (2024).[cite: 3]</li>
          <li class="pub-item">Jerin Geogy George, Kishan Dholakia, and Shanti Bhattacharya, "Generation of Bessel-like beams with reduced sidelobes for enhanced light-sheet microscopy," <em>Opt. Continuum</em> 2, 1649-1660 (2023).[cite: 3]</li>
          <li class="pub-item">Bagath Chandraprasad T, Pramitha Vayalamkuzhi, and Shanti Bhattacharya, "Transform-based phase retrieval techniques from a single off-axis interferogram," <em>Appl. Opt.</em> 60, 5523-5533 (2021).[cite: 3]</li>
          <li class="pub-item">Manu B Krishnan, Shanti Bhattacharya, Enakshi Bhattacharya, "Design and fabrication of a combined MEMS actuator and grating," <em>ISSS Journal of Micro and Smart Systems</em> 10(2), 135-143 (2021).[cite: 3]</li>
          <li class="pub-item">Isaac Nape, Nikiwe Mashaba, Nokwazi Mphuthi, Sruthy Jayakumar, Shanti Bhattacharya and Andrew Forbes, "Vector-Mode Decay in Atmospheric Turbulence: An Analysis Inspired by Quantum Mechanics," <em>Phys. Rev. Appl.</em> 15, 034030 (2021).[cite: 3]</li>
          <li class="pub-item">Amogh Manthalkar, Isaac Nape, Najmeh Tabe Bordbar, Carmelo Rosales-Guzmán, Shanti Bhattacharya, Andrew Forbes, and Angela Dudley, "All-digital Stokes polarimetry with a digital micromirror device," <em>Opt. Lett.</em> 45, 2319-2322 (2020).[cite: 3]</li>
          <li class="pub-item">Raghu Dharmavarapu, Soon Hock Ng, Fatima Eftekhari, Saulius Juodkazis, and Shanti Bhattacharya, "MetaOptics: opensource software for designing metasurface optical element GDSII layouts," <em>Opt. Express</em> 28, 3505-3516 (2020).[cite: 3]</li>
          <li class="pub-item">Sruthy J. Lathika, Vijayakumar Anand and Shanti Bhattacharya, "A compact single channel interferometer to study vortex beam propagation through scattering layers," <em>Sci Rep</em> 10, 296 (2020).[cite: 3]</li>
          <li class="pub-item">Srinivas Pachava, Raghu Dharmavarapu, Anand Vijayakumar, Sruthy Jayakumar, Amogh Manthalkar, Awakash Dixit, Nirmal K. Viswanathan, Balaji Srinivasan, Shanti Bhattacharya, "Generation and decomposition of scalar and vector modes carrying orbital angular momentum: a review," <em>Opt. Eng.</em> 59(4), 041205 (2019).[cite: 3]</li>
          <li class="pub-item">Anand, V., Bhattacharya, S. & Rosen, J., "Spatial Multiplexing Technique for Improving Dynamic Range of Speckle Correlation based Optical Lever," <em>Sci Rep</em> 9, 16035 (2019).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar, D. Jayavel, M. Muthaiah, Shanti Bhattacharya, and Joseph Rosen, "Implementation of a speckle-correlation-based optical lever with extended dynamic range," <em>Appl. Opt.</em> 58, 5982-5988 (2019).[cite: 3]</li>
          <li class="pub-item">Raghu Dharmavarapu, Ken-ichi Izumi, Ikufumi Katayama, Soon Hock Ng, Jitraporn Vongsvivut, Mark J. Tobin, Aleksandr Kuchmizhak, Yoshiaki Nishijima, Shanti Bhattacharya, and Saulius Juodkazis, "Dielectric cross-shaped resonator based metasurface for vortex beam generation in Mid-IR and THz wavelengths," <em>Nanophotonics</em> 8(7), 1263-1270 (2019).[cite: 3]</li>
          <li class="pub-item">Raghu Dharmavarapu, Shanti Bhattacharya and Saulius Juodkazis, "GDOESII: Software for design of diffractive optical elements and phase mask conversion to GDSII lithography files," <em>SoftwareX</em> 9, 126-131 (2019).[cite: 3]</li>
          <li class="pub-item">Vincent Hahn, Sebastian Kalt, Gayathri M. Sridharan, Martin Wegener and Shanti Bhattacharya, "Polarizing beam splitter integrated onto an optical fiber facet," <em>Opt. Exp.</em> 26(25), 33148-33157 (2018).[cite: 3]</li>
          <li class="pub-item">Raghu Dharmavarapu, Shanti Bhattacharya and Saulius Juodkazis, "Diffractive optics for axial intensity shaping of Bessel beams," <em>JOPT</em> 20(8), 085606 (2018).[cite: 3]</li>
          <li class="pub-item">Kavita Sharma, M. I. M. Abdul Khudus, Shaif-Ul Alam, Shanti Bhattacharya, Deepa Venkitesh, and Gilberto Brambilla, "Comparison of detection limit in fiber-based conventional, amplified, and gain-clamped cavity ring-down techniques," <em>Opt. Comm.</em> 407, 186-192 (2018).[cite: 3]</li>
          <li class="pub-item">Romita Chaudhuri, Shankar Pidishety, Shanti Bhattacharya and Balaji Srinivasan, "Design and experimental demonstration of a Fourier-domain mode-locked laser based on Erbium–doped fiber amplifier," <em>Optical Engineering</em> 56(8), 086103 (2017).[cite: 3]</li>
          <li class="pub-item">Kavita Sharma, Sijing Liang, Shaif Ul Alam, Shanti Bhattacharya, Deepa Venkitesh and Gilberto Brambilla, "Fiber-based Cavity Ring-down Technique for Refractive Index Sensing at 1953 nm using Tapered Fibers," <em>IEEE Sensors</em> (2017).[cite: 3]</li>
          <li class="pub-item">Kedar Khare, Athira Geetha and Shanti Bhattacharya, "Full resolution Fourier domain optical coherence tomography," <em>JOPT</em> (2017).[cite: 3]</li>
          <li class="pub-item">Gayathri Sridharan and Shanti Bhattacharya, "Analysis of sub-wavelength triangular gratings by simplified modal method," <em>Applied Optics</em> 55, 9712-9718 (2016).[cite: 3]</li>
          <li class="pub-item">V Pramitha, Gayathri M Sridharan and Shanti Bhattacharya, "Subwavelength transmission gratings for polarization separation in the infrared," <em>J. Micro/Nanolith. MEMS MOEMS</em> 15(2), 023504 (2016).[cite: 3]</li>
          <li class="pub-item">Pramitha Vayalamkuzhi, Shanti Bhattacharya, Ulrike Eigenthaler, Kahraman Keskinbora, C.T. Samlan, Michael Hirscher, Joachim P. Spatz and Nirmal K. Viswanathan, "Direct patterning of vortex generators on fiber tip using a focused ion beam," <em>Opt. Lett.</em> 41(10), 2133-2136 (2016).[cite: 3]</li>
          <li class="pub-item">Manu Bala Krishnan, Samuel Rosset, Shanti Bhattacharya, Herbert R. Shea, "Fabrication of transmissive dielectric elastomer actuator driven tunable optical gratings with improved tunability," <em>Opt. Eng.</em> 55(4), 047104 (2016).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar and Shanti Bhattacharya, "Compact generation of superposed first-order Bessel beams via composite diffractive optical elements," <em>Optical Engineering</em> 54(11), 111310 (2015).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar and Shanti Bhattacharya, "Design of Multi-Functional Diffractive Optical Elements," <em>Opt. Eng.</em> 54(2), 024104 (2015).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar and Shanti Bhattacharya, "Quasi-achromatic Fresnel Zone Lens with Ring Focus," <em>Appl. Opt.</em> 53(9), 1970-1974 (2014).[cite: 3]</li>
          <li class="pub-item">Suresh G. Vesalapu, Nandita DasGupta and Shanti Bhattacharya, "Digitally Tunable MOEMS Diffraction Gratings," <em>J. Micro/Nanolith. MEMS MOEMS</em> 13, 013001 (2014).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar and S. Bhattacharya, "Characterization and correction of spherical aberration due to glass substrate in the design and fabrication of Fresnel zone lenses," <em>Appl. Opt.</em> 52(24), 5932-5940 (2013).[cite: 3]</li>
          <li class="pub-item">R. Prashanth and Shanti Bhattacharya, "Improvements in speckle tracking algorithms for vibrational analysis using optical coherence tomography," <em>Journal of Biomedical Optics</em> 18(4), 046007 (2013).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar and Shanti Bhattacharya, "Design, Fabrication and Evaluation of a Multilevel Spiral Phase Fresnel Zone Plate for Optical Trapping," <em>Appl. Opt.</em> 51, 6038-6044 (2012).[cite: 3]</li>
          <li class="pub-item">M. Lai, G. Sridharan, G. Parish, S. Bhattacharya and A. Keating, "Multilayer porous silicon diffraction gratings operating in the infrared," <em>Nanoscale Research Lett.</em> 7:645 (2012).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar and Shanti Bhattacharya, "Phase shifted Fresnel Axicon," <em>Opt. Lett.</em> 37, 1980-1982 (2012).[cite: 3]</li>
          <li class="pub-item">A. Kulkarni, G Lakshminarayan, S. Bhattacharya and Anil Prabhakar, "All fibre interferometry: Control and error analysis," <em>Appl. Optics</em> 50, 4450–4456 (2011).[cite: 3]</li>
          <li class="pub-item">Deepak K Agrawal and Shanti Bhattacharya, "Integrated Optical and MEMS based Design Process for a Variable Optical Attenuator," <em>Opt. And Lasers in Engg.</em> 49, 848-854 (2011).[cite: 3]</li>
          <li class="pub-item">K. A. G. Prakash, S. Dhabai, E. Bhattacharya and S. Bhattacharya, "Design and Fabrication of a Micro-mirror for Low Resolution Spectroscopy," <em>IEEE Sensors</em> 11, 1019-1025 (2011).[cite: 3]</li>
          <li class="pub-item">Khansa C.A, Shanti Bhattacharya, Anil Prabhakar, "Multiwavelength Erbium Doped Fiber Ring Lasers," <em>Opt. Commun</em> 282, 2380–2387 (2009).[cite: 3]</li>
          <li class="pub-item">S. Bhattacharya, "Simplified Mesh Techniques for Design of Beam Shaping Diffractive Optical Elements," <em>Optik</em> 119, 321–328 (2008).[cite: 3]</li>
          <li class="pub-item">S. Bhattacharya and A. Hartzell, "Optical microelectromechanical systems: designing for reliability," <em>J. Micro/Nanolith. MEMS MOEMS</em> 6, 033010 (2007).[cite: 3]</li>
          <li class="pub-item">S. Stankovic et al., "Integrated optical pickup system for axial dual focus," <em>Appl. Optics</em> 40, 614-621 (2001).[cite: 3]</li>
          <li class="pub-item">M. Hain et al., "Fast switching liquid crystal lenses for a dual focus digital versatile disc pickup," <em>Opt. Comm.</em> 188, 291-299 (2001).[cite: 3]</li>
          <li class="pub-item">S. Bhattacharya, L.L. Wang, T. Tschudi, R. S. Sirohi, "Optical perfect shuffle using diffractive optical elements," <em>Optik</em> 110, 233-237 (1999).[cite: 3]</li>
          <li class="pub-item">S. Bhattacharya, V. V. Rao and R. S. Sirohi, "Phase checker grating as an array illuminator," <em>Optik</em> 106, 15-18 (1997).[cite: 3]</li>
          <li class="pub-item">S. Bhattacharya and R. S. Sirohi, "Amplitude checker grating from 1-D Ronchi grating and its application to array generation," <em>Appl. Opt.</em> 36, 3745-3752 (1997).[cite: 3]</li>
          <li class="pub-item">J. S. Darlin, P. Senthilkumaran, S. Bhattacharya, M. P. Kothiyal and R. S. Sirohi, "Fabrication of array illuminator using Michelson interferometers in tandem," <em>Opt. Commun.</em> 123, 1-4 (1996).[cite: 3]</li>
          <li class="pub-item">S. Bhattacharya, J. S. Darlin, P. Senthilkumaran, M. P. Kothiyal and R. S. Sirohi, "Holographic array illuminator using Michelson interferometers in tandem: Fabrication and analysis," <em>J. Mod. Opt.</em> 42, 2275-2283 (1995).[cite: 3]</li>
        </ul>
      </div>
    </details>

    <!-- 3. NATIONAL JOURNALS -->
    <details class="collapsible-section">
      <summary class="collapsible-header">National Journals</summary>
      <div class="pub-content">
        <ul class="pub-list">
          <li class="pub-item">Jerin Geogy George, Susan Thomas and Shanti Bhattacharya, "Design of multi-wavelength dielectric metasurfaces using finite element software," <em>Asian Journal of Physics</em> 30(4), April 2021.[cite: 3]</li>
          <li class="pub-item">V. Pramitha and Shanti Bhattacharya, "Focused ion beam milling for the fabrication of beam-shaping spiral phase optical elements," <em>Asian J Phys</em> 25(7), 2016.[cite: 3]</li>
          <li class="pub-item">Raghu Dharmavarapu, A. Vijayakumar and Shanti Bhattacharya, "Design and Fabrication of Holographic Optical Elements for the Generation of Tilted and Accelerating Airy Beams," <em>Asian Journal of Physics</em> 24(10), 1363-1371 (2015).[cite: 3]</li>
          <li class="pub-item">A. Vijayakumar, Gayathri M. Sridharan, M. Karthickraj and Shanti Bhattacharya, "Design, Fabrication and Evaluation of a Multilevel Fraxicon," <em>AJP</em> 23(5), (2014).[cite: 3]</li>
          <li class="pub-item">S. Bhattacharya, V. V. Rao and R. S. Sirohi, "Array generators: A Review," <em>J. of Optics, India</em> 25, 203-221 (1996).[cite: 3]</li>
        </ul>
      </div>
    </details>

    <!-- 4. CONFERENCES -->
    <details class="collapsible-section">
      <summary class="collapsible-header">Conferences</summary>
      <div class="pub-content">

        <!-- 4a. International Conferences -->
        <details class="nested-collapsible" open>
          <summary class="nested-header">International Conferences</summary>
          <div class="pub-content">
            <ul class="pub-list">
              <li class="pub-item">M. F. Kabir, J. G. George, S. Bhattacharya, and S. Ramachandran, "Generation of Bottle Beams with a Single Metasurface," <em>CLEO 2026</em>, Long Beach, California, May 2026.[cite: 3]</li>
              <li class="pub-item">Susan Thomas, Francesco Ferranti and Shanti Bhattacharya, "Metaelement enhanced confocal scanning fiber fluorescence endoscopy optical system," <em>SPIE Photonics West 2026</em>, San Francisco, January 2026.[cite: 3]</li>
              <li class="pub-item">N. K. Pothapakula and Shanti Bhattacharya, "OCT based investigation of post harvest sub-peel micro-structural changes in Mango (Mangifera indica)," <em>SPIE Photonics West 2026</em>, San Francisco, January 2026.[cite: 3]</li>
              <li class="pub-item">Shanti Bhattacharya, "Optimising Metasurface Design and Fabrication for Microendoscopy," <em>OPTIQ 2025</em>, CUSAT, Kochi, November 2025.[cite: 3]</li>
              <li class="pub-item">Shanti Bhattacharya, "Modified Bessel Beams and their Applications," <em>International Conference on Applied Physics and Imaging</em>, Tartu, Estonia, September 2025.[cite: 3]</li>
              <li class="pub-item">Jerin Geogy George and Shanti Bhattacharya, "Far-Field Spatial Filtering for Enhanced Bessel Light Sheets Generated Using Silicon Nitride Metasurfaces," <em>Optical Design and Fabrication Congress</em>, Denver, June 2025.[cite: 3]</li>
              <li class="pub-item">Susan Thomas, Hira Nayak, Francesco Ferranti, and Shanti Bhattacharya, "Metaoptics for Aberration Correction in Fluorescence Imaging Endoscopy Optical Systems," <em>Optical Design and Fabrication Congress</em>, Denver, June 2025.[cite: 3]</li>
              <li class="pub-item">Mathu Mathi Murugavel and Shanti Bhattacharya, "Diffuse reflection collection optics for analyzing chicory content in coffee," <em>SPIE Photonics West 2025</em>, San Francisco, January 2025.[cite: 3]</li>
              <li class="pub-item">Susan Thomas, Francesco Ferranti, and Shanti Bhattacharya, "Model and evaluation of illumination and collection in a metasurface integrated imaging probe for endoscopy," <em>ETOT-I</em>, SRM University, AP, January 2025.[cite: 3]</li>
              <li class="pub-item">Bagath Chandraprasad T, Manu Bala Krishnan, Pramitha V, and Shanti Bhattacharya, "Characterization of an Optical MEMS device employing Optical Phase Retrieval technique," <em>ETOT-I</em>, AP, January 2025.[cite: 3]</li>
              <li class="pub-item">N. K. Pothapakula, S. Bhattacharya, "Wigner Ville Distribution assisted spectral domain OCT for high resolution rice leaf structural imaging at 1550 nm," <em>ETOT-I</em>, SRM, AP, January 2025.[cite: 3]</li>
              <li class="pub-item">Jerin Geogy George, and Shanti Bhattacharya, "Mitigating Tailing Effects in Digitally Scanned Bessel Beams for Light Sheet Imaging," <em>ETOT-I</em>, AP, January 2025.[cite: 3]</li>
              <li class="pub-item">Jerin Geogy George, Shanti Bhattacharya and Kishan Dholakia, "Structured Illumination Using Modified Bessel Beams with Reduced Sidelobes," <em>CLEO PR</em>, Incheon, Korea, August 2024.[cite: 3]</li>
              <li class="pub-item">Susan Thomas and Shanti Bhattacharya, "Compact and portable scanning fiber-optic confocal microendoscopy system for reflectance and fluorescence imaging," <em>SPIE Optical System Design</em>, Strasbourg, April 2024.[cite: 3]</li>
              <li class="pub-item">Susan Thomas, Francesco Ferranti, Shanti Bhattacharya, "Design and simulation of dielectric metasurfaces for aberration correction in fiber-scanning microendoscope," <em>SPIE PW</em>, San Francisco, 2024.[cite: 3]</li>
              <li class="pub-item">Naveen Kumar Pothapakula, Ravinder David Koilpillai, Shanti Bhattacharya, "Optical signal processing in spectral domain OCT using smoothed pseudo Wigner-Ville distribution," <em>SPIE PW</em>, San Francisco, 2024.[cite: 3]</li>
              <li class="pub-item">Sreeraj P. Nambiar, Susan Thomas, Shanti Bhattacharya, Enakshi Bhattacharya, "Design and fabrication of an electrothermally-actuated 2D scanning micromirror," <em>SPIE PW</em>, San Francisco, 2024.[cite: 3]</li>
              <li class="pub-item">Mathu Mathi Murugavel and Shanti Bhattacharya, "Design and Testing of Diffuse Reflection Collection Optics for Vis-NIR Spectroscopy for Soil Analysis," <em>Photonics 2023</em>, IISc Bengaluru, July 2023.[cite: 3]</li>
              <li class="pub-item">Susan Thomas and Shanti Bhattacharya, "Reflectance Imaging with Double Clad Fiber Coupler and Micro-Optics for Confocal Endoscopy," <em>Photonics 2023</em>, IISc Bengaluru, July 2023.[cite: 3]</li>
              <li class="pub-item">Jerin Geogy George, and Shanti Bhattacharya, "Engineering Axial Intensity of Bessel Beams Using Meta-Axicons with Amplitude and Phase Control," <em>Photonics 2023</em>, IISc Bengaluru, July 2023.[cite: 3]</li>
              <li class="pub-item">Sreeraj P Nambiar, Meenakshi Rajasekaran, Shanti Bhattacharya and Enakshi Bhattacharya, "Design of an Electrothermally Actuated MEMS Mirror for a Two Photon Fluorescence Micro-Endoscope," <em>Photonics 2023</em>, IISc Bengaluru, July 2023.[cite: 3]</li>
              <li class="pub-item">Bagath Chandraprasad T, Pramitha Vayalamkuzhi and Shanti Bhattacharya, "Study on pre-filtering requirements of Hilbert transform method for optical phase retrieval," <em>SPIE PW</em>, 2023.[cite: 3]</li>
              <li class="pub-item">Susan Thomas and Shanti Bhattacharya, "Optical design and simulation of two photon fluorescence imaging microendoscope with aberration correction," <em>SPIE PW</em>, 2023.[cite: 3]</li>
              <li class="pub-item">Atreyee Saha et al., "LWGNet - Learned Wirtinger Gradients for Fourier Ptychographic Phase Retrieval," <em>ECCV</em>, Tel Aviv, Oct. 2022.[cite: 3]</li>
              <li class="pub-item">N. Pothapakula and S. Bhattacharya, "Continuous wavelet transformations for OCT image reconstruction: Applications," <em>Frontiers in Optics + Laser Science 2022</em>, NY, USA, Oct. 2022.[cite: 3]</li>
              <li class="pub-item">Jerin Geogy George, Yerragadda Guruvaiah and Shanti Bhattacharya, "Sidelobe-Suppressed Bessel Beam using Holograms," <em>CLEO PR</em>, Sapporo, Japan, 2022.[cite: 3]</li>
              <li class="pub-item">Jerin G. George, Francesco Ferranti and Shanti Bhattacharya, "Design and Fabrication of dielectric meta-optics for beam-shaping," <em>2nd Annual International Scientific Conference on Lasers, Optics, Photonics, Sensors & Ultrafast Nonlinear Optics</em>, June 2022.[cite: 3]</li>
              <li class="pub-item">G. Yerragadda, Raghu Dharmavarapu, Saulius Juodkazis and Shanti Bhattacharya, "Design and optimized fabrication techniques for highly-efficient dielectric meta-optical airy beam generators," <em>SPIE PW</em>, 2021.[cite: 3]</li>
              <li class="pub-item">B. Chandraprasad T, P. Vayalamkuzhi and S. Bhattacharya, "Optical Phase Extraction using Fourier, Continuous Wavelet and Hilbert Transform Methods," <em>CLEO-PR</em>, August 2020.[cite: 3]</li>
              <li class="pub-item">Raghu Dharmavarapu et al., "MetaOptics: Software for designing metasurface optical elements," <em>ICOL - 2019</em>, Dehradun, Oct 2019. (Best paper award)[cite: 3]</li>
              <li class="pub-item">Shanti Bhattacharya, A. Vijayakumar, Sruthy J Lathika and J. Rosen, "Speckle Correlation Technique to Improve the Dynamic Range of an Optical Lever," <em>Laser Congress</em>, Vienna, Austria, 2019.[cite: 3]</li>
              <li class="pub-item">Sruthy J Lathika, A Vijayakumar and Shanti Bhattacharya, "Compact Single-channel Interferometer for the Study of Light Propagation through Thin Diffusers," <em>Laser Congress</em>, Vienna, Austria, 2019.[cite: 3]</li>
            </ul>
          </div>
        </details>

        <!-- 4b. National Conferences -->
        <details class="nested-collapsible">
          <summary class="nested-header">National Conferences</summary>
          <div class="pub-content">
            <ul class="pub-list">
              <li class="pub-item">Mathu Mathi Murugavel, Shanti Bhattacharya, "Design of a low cost and compact near infrared spectrometer for powder sample analysis," <em>Proc. SPIE 13108, Women in Optics and Photonics in India 2023</em>, 131080D (Jan 2024).[cite: 3]</li>
              <li class="pub-item">A. Suresh and S. Bhattacharya, "Design of a Hybrid Eyepiece for a See-through Head Mounted Display," <em>Optical Society of India Symposium</em>, Tezpur University, Assam, Dec. 2007.[cite: 3]</li>
              <li class="pub-item">A. Suresh and S. Bhattacharya, "Design and comparison of refractive and hybrid eyepieces," <em>National Conference on Recent Trends in Optoelectronics and Laser Technology</em>, Trivandrum, April 2007.[cite: 3]</li>
              <li class="pub-item">C. A. Khansa, S. Bhattacharya and A. Prabhakar, "Four wavelength Erbium Doped Fibre Laser," <em>Nat. Conf. On recent trends in Optoelectronics and Lasers</em>, Trivandrum, April 2007.[cite: 3]</li>
              <li class="pub-item">S. Bhattacharya, V. V. Rao and R. S. Sirohi, "Holographic array illuminators in partially coherent light," <em>National Symposium of the Optical Society of India</em>, IRDE, Dehra Dun, March 1996.[cite: 3]</li>
              <li class="pub-item">S. Bhattacharya, V. V. Rao and R.S. Sirohi, "Array generation using checker gratings and the Talbot effect," <em>National Laser Symposium</em>, BARC, Bombay, January 1996.[cite: 3]</li>
              <li class="pub-item">S. Bhattacharya, J. S. Darlin, P. Senthilkumaran, M. P. Kothiyal and R. S. Sirohi, "Study of interferometric array generators with different levels of phase modulation," <em>National Symposium of the Optical Society of India</em>, CSIO, Chandigarh, March 1995.[cite: 3]</li>
            </ul>
          </div>
        </details>

      </div>
    </details>

    <!-- 5. PATENTS -->
    <details class="collapsible-section">
      <summary class="collapsible-header">Patents</summary>
      <div class="pub-content">
        <ul class="pub-list">
          <li class="pub-item">
            <strong>An imaging system and a method for Fourier Ptychographic Microscopy (FPM)</strong><br>
            Kaushik Mitra, Shanti Bhattacharya, Atreyee Saha, Salman Siddique Khan, Sagar Sehrawat, Sanjana Santosh Prabhu and Aindra Systems Pvt. Ltd.<br>
            <em>Patent No.: 423241</em> | Filed: 19/07/2022 | Granted: July 19, 2023[cite: 3]
          </li>
          <li class="pub-item">
            <strong>System and method for full resolution Fourier Domain OCT imaging</strong><br>
            Kedar B. Khare and Shanti Bhattacharya<br>
            <em>Patent No.: 446657</em> | Filed: April 07, 2017 | Granted: September 23, 2023[cite: 3]
          </li>
          <li class="pub-item">
            <strong>Fibre-attached optical switch with in-plane micro-machined mirrors</strong><br>
            C. Yun, S. Bhattacharya et al.<br>
            <em>Patent No.: 6,931,170B2</em> | Issued: August 16, 2005[cite: 3]
          </li>
          <li class="pub-item">
            <strong>Method and Apparatus for optical Switching with same side input and outputs</strong><br>
            Shanti Bhattacharya and Jeff Swift<br>
            <em>Patent No.: 6,842,555</em> | Issued: January 11, 2005[cite: 3]
          </li>
        </ul>
      </div>
    </details>

    <!-- 6. INVITED LECTURES AND ARTICLES -->
    <details class="collapsible-section">
      <summary class="collapsible-header">Invited Lectures and Articles</summary>
      <div class="pub-content">
        <ul class="pub-list">
          <li class="pub-item">Shanti Bhattacharya, "Metaoptics for endoscopy," MEDIT, RWTH Aachen, Germany, July 1, 2026.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Metaoptics for endoscopy," BTU Cottbus-Senftenberg, Cottbus, June 23, 2026.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Manipulated Bessel Beams and their Applications," Physics Colloquium, BTU Cottbus-Senftenberg, June 5, 2025.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Metaoptics for endoscopy," IHP, Frankfurt (Oder) Germany, June 3, 2025.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Multi-pronged approach to improving Imaging: better algorithms, complex light, and nano-photonics," (Invited talk), ETOT-I, Vijayawada, January 2-4, 2025.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Light Camera Action!", Public lecture by AIP (SA branch) and Adelaide Optics Chapter, November 18, 2024.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Generation of Sidelobe Suppressed Bessel Beams for Imaging," (Invited talk), Univ. of Adelaide, November 15, 2024.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Meta-optics for Generation of Sidelobe-Suppressed Bessel Beams," (Invited talk), OPTOIn-2024, Chandigarh, October 23–25, 2024.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Controlling light using nanophotonics," (Invited talk), SCOP Students Conference, PRL, Ahmedabad, September 25–27, 2024.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Nano and micro optics on fibre tip: A possible solution for measurements in harsh environments," (Invited talk), IMEC2024, Belgrade, Serbia, March 20–22, 2024.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Manipulating Light with Micro and Nano-Optics," IIITDM Kancheepuram, September 22, 2023.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Multi-functional Diffractive and meta-optics for light manipulation," Univ. of Adelaide, March 23, 2023.[cite: 3]</li>
          <li class="pub-item">Enakshi Bhattacharya, Nandita DasGupta and Shanti Bhattacharya, "Optical MEMS at IIT Madras," (Invited talk), MAMM 2022, IIT Hyderabad, December 3-5, 2022.[cite: 3]</li>
          <li class="pub-item">Jerin Geogy George, Susan Thomas, and Shanti Bhattacharya, "Design and Fabrication of Meta-optics for Light Manipulation: Challenges and Prospects," (Invited talk), OSI COPaQ 2022, IIT Roorkee, November 10-13, 2022.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Small Optic, Infinite Possibilities," IITMAA GuruTalks, September 23, 2022. <a href="https://youtu.be/OJyH-6eYIt4" target="_blank">Watch Video</a>[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Light manipulation - the Nano-optics Way," National Science Day 2022, St. Pauls College, Kalamassery, February 26, 2022.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, Interview for Optics & Photonics News (OPN), June 2021.[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Want to come on a journey with me? I travel light," IEEE Women in Photonics Spotlight Lecture, March 8, 2021. <a href="https://bit.ly/3rxZbA6" target="_blank">Lecture Link</a>[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Shrinking Optics, Expanding Possibilities," Photonics Colloquium, OSA IITM Student Chapter, July 31, 2020. <a href="https://youtu.be/VYTO5H_2yMQ" target="_blank">Watch Video</a>[cite: 3]</li>
          <li class="pub-item">Shanti Bhattacharya, "Including reliability in the design of optical micro electro mechanical systems," <em>SPIE Newsroom</em>, May 2007.[cite: 3]</li>
        </ul>
      </div>
    </details>

  </div>
</div>
