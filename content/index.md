---
title: "[ADDRESS]"
description: "A rare offering at [ADDRESS] — [BEDS] beds, [BATHS] baths, [SQFT] sq ft, offered at [PRICE]."
cssclasses:
  - luxury-listing
---

<!--
  ============================================================
  LUXURY LISTING SITE — CONTENT GUIDE
  ============================================================
  This single page contains every section of the brochure site.
  Search for the bracket tokens below and replace with real content:

    [ADDRESS]        → property street address / listing name
    [PRICE]           → asking price
    [BEDS] [BATHS] [SQFT] [LOT SIZE] → key stats
    [PLACEHOLDER PARAGRAPH] → editorial listing description copy
    [AGENT NAME] [BROKERAGE] [PHONE] [EMAIL] → agent/contact info
    [MLS#]            → MLS disclosure number
    YOUR_FORMSPREE_ID → replace in the contact form action URL
    Map query string  → replace the address in the Google Maps iframe src

  PHOTOS: every gallery/hero/floor-plan image is currently a placeholder
  <div class="photo-placeholder"> with a data-label describing exactly
  which photo goes there. To swap in a real photo, replace the placeholder
  div's contents with an <img src="..." alt="..." loading="lazy"> — the
  surrounding container already has the correct aspect-ratio set in
  quartz/styles/custom.scss, so no layout/CSS changes are needed.
  ============================================================
-->

<nav id="site-nav" class="ll-nav">
  <a href="#hero" class="ll-nav__brand">[ADDRESS]</a>
  <button id="navToggle" class="ll-nav__toggle" aria-label="Toggle navigation" aria-expanded="false">
    <span></span><span></span><span></span>
  </button>
  <div class="ll-nav__links" id="navLinks">
    <a href="#hero">Home</a>
    <a href="#gallery">Gallery</a>
    <a href="#features">Features</a>
    <a href="#location">Location</a>
    <a href="#contact">Contact</a>
  </div>
</nav>

<section id="hero" class="ll-hero reveal">
  <!-- Swap: replace with full-bleed exterior hero photo (e.g. background-image on .ll-hero, or an <img> behind the overlay) -->
  <div class="ll-hero__placeholder photo-placeholder" data-label="Hero — Exterior, Twilight">
    <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
    <span class="ph-label">Hero — Exterior, Twilight</span>
  </div>
  <div class="ll-hero__scrim"></div>
  <div class="ll-hero__content">
    <p class="ll-hero__eyebrow">Offered at [PRICE]</p>
    <h1 class="ll-hero__title">[ADDRESS]</h1>
    <p class="ll-hero__subtitle">[BEDS] Beds &nbsp;·&nbsp; [BATHS] Baths &nbsp;·&nbsp; [SQFT] Sq Ft</p>
  </div>
  <a href="#overview" class="ll-hero__scroll-cue" aria-label="Scroll to explore">
    <span>Scroll to Explore</span>
    <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 4v15M5 12l7 7 7-7" /></svg>
  </a>
</section>

<section id="overview" class="ll-section reveal">
  <div class="ll-container">
    <div class="ll-stats">
      <div class="ll-stat">
        <span class="ll-stat__value">[PRICE]</span>
        <span class="ll-stat__label">Asking Price</span>
      </div>
      <div class="ll-stat">
        <span class="ll-stat__value">[BEDS]</span>
        <span class="ll-stat__label">Bedrooms</span>
      </div>
      <div class="ll-stat">
        <span class="ll-stat__value">[BATHS]</span>
        <span class="ll-stat__label">Bathrooms</span>
      </div>
      <div class="ll-stat">
        <span class="ll-stat__value">[SQFT]</span>
        <span class="ll-stat__label">Square Feet</span>
      </div>
      <div class="ll-stat">
        <span class="ll-stat__value">[LOT SIZE]</span>
        <span class="ll-stat__label">Lot Size</span>
      </div>
    </div>
    <div class="ll-description">
      <h2 class="ll-eyebrow-heading">The Property</h2>
      <!-- Swap: replace this paragraph with real editorial listing copy, roughly 100–150 words -->
      <p>[PLACEHOLDER PARAGRAPH]</p>
    </div>
  </div>
</section>

<section id="gallery" class="ll-section ll-section--alt reveal">
  <div class="ll-container">
    <h2 class="ll-eyebrow-heading">Gallery</h2>
    <h3 class="ll-gallery__group-title">Exterior</h3>
    <div class="ll-gallery">
      <button class="photo-placeholder ll-photo" data-label="Exterior — Front Facade" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Exterior — Front Facade</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Exterior — Rear &amp; Pool" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Exterior — Rear &amp; Pool</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Exterior — Aerial View" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Exterior — Aerial View</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Exterior — Entry &amp; Motor Court" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Exterior — Entry &amp; Motor Court</span>
      </button>
    </div>
    <h3 class="ll-gallery__group-title">Kitchen</h3>
    <div class="ll-gallery">
      <button class="photo-placeholder ll-photo" data-label="Kitchen — Main View" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Kitchen — Main View</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Kitchen — Island &amp; Range" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Kitchen — Island &amp; Range</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Kitchen — Breakfast Nook" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Kitchen — Breakfast Nook</span>
      </button>
    </div>
    <h3 class="ll-gallery__group-title">Living Spaces</h3>
    <div class="ll-gallery">
      <button class="photo-placeholder ll-photo" data-label="Living — Great Room" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Living — Great Room</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Living — Family Room" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Living — Family Room</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Living — Formal Dining" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Living — Formal Dining</span>
      </button>
    </div>
    <h3 class="ll-gallery__group-title">Primary Suite</h3>
    <div class="ll-gallery">
      <button class="photo-placeholder ll-photo" data-label="Primary Suite — Bedroom" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Primary Suite — Bedroom</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Primary Suite — Ensuite Bath" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Primary Suite — Ensuite Bath</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Primary Suite — Walk-in Closet" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Primary Suite — Walk-in Closet</span>
      </button>
    </div>
    <h3 class="ll-gallery__group-title">Outdoor &amp; Amenities</h3>
    <div class="ll-gallery">
      <button class="photo-placeholder ll-photo" data-label="Outdoor — Pool &amp; Spa" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Outdoor — Pool &amp; Spa</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Outdoor — Covered Patio" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Outdoor — Covered Patio</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Outdoor — Guest House" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Outdoor — Guest House</span>
      </button>
      <button class="photo-placeholder ll-photo" data-label="Outdoor — Gardens" type="button">
        <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 16.5 8.5 10l3.5 4 3-4L20 16.5" /><circle cx="12" cy="12" r="9.25" /></svg>
        <span class="ph-label">Outdoor — Gardens</span>
      </button>
    </div>
  </div>
</section>

<section id="features" class="ll-section reveal">
  <div class="ll-container">
    <h2 class="ll-eyebrow-heading">Features &amp; Amenities</h2>
    <div class="ll-features">
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><circle cx="12" cy="12" r="9" /><path d="M12 7v5l3 2" /></svg>
        <h3>Architectural Pedigree</h3>
        <p>[Notable architect / design style / year built]</p>
      </div>
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M4 20v-8l8-6 8 6v8" /><path d="M9 20v-6h6v6" /><path d="M6.5 10.5a8 8 0 0 1 11 0" /></svg>
        <h3>Smart Home Integration</h3>
        <p>[Automated lighting, climate, security, and audio systems]</p>
      </div>
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M12 3l1.8 4.6L18 9l-4.2 1.4L12 15l-1.8-4.6L6 9l4.2-1.4z" /></svg>
        <h3>Chef's Kitchen &amp; Premium Finishes</h3>
        <p>[Imported stone, custom millwork, professional-grade appliances]</p>
      </div>
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><rect x="4" y="10" width="16" height="7" rx="1.5" /><path d="M6 10V8a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v2" /><path d="M4 17v2M20 17v2" /></svg>
        <h3>Primary Suite Retreat</h3>
        <p>[Spa-style bath, dual walk-in closets, private balcony]</p>
      </div>
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><circle cx="12" cy="12" r="4" /><path d="M12 2v3M12 19v3M4.2 4.2l2.1 2.1M17.7 17.7l2.1 2.1M2 12h3M19 12h3M4.2 19.8l2.1-2.1M17.7 6.3l2.1-2.1" /></svg>
        <h3>Resort-Style Outdoor Living</h3>
        <p>[Pool, spa, outdoor kitchen, mature landscaping]</p>
      </div>
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M6 20V10l6-6 6 6v10" /><path d="M9 20v-5a3 3 0 0 1 6 0v5" /></svg>
        <h3>Wine Cellar &amp; Bespoke Millwork</h3>
        <p>[Climate-controlled cellar, custom built-ins]</p>
      </div>
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M3 13l2-5a2 2 0 0 1 2-1h10a2 2 0 0 1 2 1l2 5" /><rect x="3" y="13" width="18" height="6" rx="1.5" /><circle cx="7.5" cy="19" r="1.2" /><circle cx="16.5" cy="19" r="1.2" /></svg>
        <h3>Three-Car Garage &amp; Motor Court</h3>
        <p>[Garage details, guest parking, gated entry]</p>
      </div>
      <div class="ll-feature">
        <svg class="ll-feature__icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M12 3l7 3v6c0 4.5-3 7.5-7 9-4-1.5-7-4.5-7-9V6z" /></svg>
        <h3>Privacy &amp; Security</h3>
        <p>[Gated access, security systems, mature perimeter landscaping]</p>
      </div>
    </div>
  </div>
</section>

<section id="floorplan" class="ll-section ll-section--alt reveal">
  <div class="ll-container">
    <h2 class="ll-eyebrow-heading">Floor Plan</h2>
    <!-- Swap: replace with the actual floor plan image, ideally with labeled rooms -->
    <div class="photo-placeholder ll-floorplan" data-label="Floor Plan — Main Level">
      <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><rect x="3" y="3" width="18" height="18" rx="1" /><path d="M3 9h18M9 9v12M15 3v6" /></svg>
      <span class="ph-label">Floor Plan — Main Level</span>
    </div>
    <p class="ll-floorplan__note">[Add room-by-room breakdown or a second floor plan for additional levels]</p>
  </div>
</section>

<section id="tour" class="ll-section reveal">
  <div class="ll-container">
    <h2 class="ll-eyebrow-heading">Virtual Tour</h2>
    <!--
      Swap: replace this placeholder with an embedded video or Matterport 3D tour, e.g.:
      <div class="ll-tour__frame">
        <iframe src="https://my.matterport.com/show/?m=YOUR_MODEL_ID" allowfullscreen loading="lazy"></iframe>
      </div>
    -->
    <div class="photo-placeholder ll-tour__frame" data-label="Virtual Tour — Add Matterport or Video Embed">
      <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><circle cx="12" cy="12" r="9" /><path d="M10 8.5v7l6-3.5z" /></svg>
      <span class="ph-label">Virtual Tour — Add Matterport or Video Embed</span>
    </div>
  </div>
</section>

<section id="location" class="ll-section ll-section--alt reveal">
  <div class="ll-container">
    <h2 class="ll-eyebrow-heading">Location</h2>
    <div class="ll-location">
      <!-- Swap: replace the q= value with the real property address, keep &output=embed (no API key required) -->
      <div class="ll-location__map">
        <iframe
          src="https://www.google.com/maps?q=[ADDRESS]&output=embed"
          width="100%"
          height="420"
          style="border:0"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
          title="Property location map">
        </iframe>
      </div>
      <div class="ll-location__info">
        <p>[Neighborhood blurb — a few sentences on the area, character, and lifestyle]</p>
        <ul class="ll-poi">
          <li><span>[X] min</span> to [Nearby landmark or town center]</li>
          <li><span>[X] min</span> to [Nearby beach / park / trailhead]</li>
          <li><span>[X] min</span> to [Nearby shopping / dining district]</li>
          <li><span>[X] min</span> to [Nearest airport]</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="contact" class="ll-section reveal">
  <div class="ll-container ll-container--narrow">
    <h2 class="ll-eyebrow-heading">Inquire</h2>
    <div class="ll-contact">
      <div class="ll-contact__agent">
        <div class="photo-placeholder ll-contact__photo" data-label="Agent Headshot">
          <svg class="ph-icon" viewBox="0 0 24 24" aria-hidden="true"><circle cx="12" cy="8.5" r="4" /><path d="M4.5 20a7.5 7.5 0 0 1 15 0" /></svg>
          <span class="ph-label">Agent Headshot</span>
        </div>
        <h3>[AGENT NAME]</h3>
        <p class="ll-contact__brokerage">[BROKERAGE]</p>
        <p><a href="tel:[PHONE]">[PHONE]</a></p>
        <p><a href="mailto:[EMAIL]">[EMAIL]</a></p>
      </div>
      <!-- Swap: replace YOUR_FORMSPREE_ID with your real Formspree form ID (formspree.io) -->
      <form class="ll-form" action="https://formspree.io/f/YOUR_FORMSPREE_ID" method="POST">
        <label>
          Name
          <input type="text" name="name" required />
        </label>
        <label>
          Email
          <input type="email" name="email" required />
        </label>
        <label>
          Phone
          <input type="tel" name="phone" />
        </label>
        <label>
          Message
          <textarea name="message" rows="4" placeholder="I'd like to schedule a private showing of [ADDRESS]."></textarea>
        </label>
        <button type="submit" class="ll-btn">Request a Private Showing</button>
        <p class="ll-form__fallback">Prefer email? Reach us directly at <a href="mailto:[EMAIL]">[EMAIL]</a>.</p>
      </form>
    </div>
  </div>
</section>

<footer class="ll-footer">
  <div class="ll-container">
    <p class="ll-footer__disclaimer">
      [MLS#] · Information deemed reliable but not guaranteed. Square footage, lot size, and other
      details are approximate and should be independently verified. Offered by [BROKERAGE].
      Equal Housing Opportunity.
    </p>
    <div class="ll-footer__row">
      <p>&copy; <span id="year"></span> [BROKERAGE]. All rights reserved.</p>
      <div class="ll-footer__social">
        <a href="#" aria-label="Instagram">[Instagram]</a>
        <a href="#" aria-label="Facebook">[Facebook]</a>
        <a href="#" aria-label="LinkedIn">[LinkedIn]</a>
      </div>
    </div>
  </div>
</footer>

<script>
(function () {
  // Sticky nav: transparent over hero, solid once scrolled
  var nav = document.getElementById("site-nav");
  var hero = document.getElementById("hero");
  function updateNav() {
    if (!nav || !hero) return;
    var threshold = hero.offsetHeight * 0.7;
    if (window.scrollY > threshold) {
      nav.classList.add("is-solid");
    } else {
      nav.classList.remove("is-solid");
    }
  }
  document.addEventListener("scroll", updateNav, { passive: true });
  updateNav();

  // Mobile nav toggle
  var toggle = document.getElementById("navToggle");
  var links = document.getElementById("navLinks");
  if (toggle && links) {
    toggle.addEventListener("click", function () {
      var open = links.classList.toggle("is-open");
      toggle.setAttribute("aria-expanded", open ? "true" : "false");
    });
    links.querySelectorAll("a").forEach(function (link) {
      link.addEventListener("click", function () {
        links.classList.remove("is-open");
        toggle.setAttribute("aria-expanded", "false");
      });
    });
  }

  // Scroll-triggered fade/slide reveal
  var revealEls = document.querySelectorAll(".reveal");
  if ("IntersectionObserver" in window) {
    var observer = new IntersectionObserver(
      function (entries) {
        entries.forEach(function (entry) {
          if (entry.isIntersecting) {
            entry.target.classList.add("is-visible");
            observer.unobserve(entry.target);
          }
        });
      },
      { threshold: 0.12 }
    );
    revealEls.forEach(function (el) { observer.observe(el); });
  } else {
    revealEls.forEach(function (el) { el.classList.add("is-visible"); });
  }

  // Lightbox for gallery + floor plan + hero placeholders
  var lightbox = document.createElement("div");
  lightbox.className = "ll-lightbox";
  lightbox.innerHTML =
    '<button class="ll-lightbox__close" aria-label="Close">&times;</button>' +
    '<div class="ll-lightbox__inner"></div>';
  document.body.appendChild(lightbox);

  function openLightbox(sourceEl) {
    var inner = lightbox.querySelector(".ll-lightbox__inner");
    inner.innerHTML = sourceEl.innerHTML;
    lightbox.classList.add("is-open");
    document.body.style.overflow = "hidden";
  }
  function closeLightbox() {
    lightbox.classList.remove("is-open");
    document.body.style.overflow = "";
  }
  lightbox.addEventListener("click", function (e) {
    if (e.target === lightbox || e.target.classList.contains("ll-lightbox__close")) {
      closeLightbox();
    }
  });
  document.addEventListener("keydown", function (e) {
    if (e.key === "Escape") closeLightbox();
  });
  document.querySelectorAll(".ll-photo").forEach(function (el) {
    el.addEventListener("click", function () { openLightbox(el); });
  });

  // Footer year
  var yearEl = document.getElementById("year");
  if (yearEl) yearEl.textContent = new Date().getFullYear();
})();
</script>
