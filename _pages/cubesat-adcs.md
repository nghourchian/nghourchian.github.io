---
layout: single
title: "Attitude Determination and Control System"
permalink: /projects/cubesat-adcs/
author_profile: false
---

<style>
.page__content {
  padding-top: 1.5rem;
}

/* =========================
   Announcement cards
   ========================= */

.cubesat-news-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 360px));
  justify-content: center;
  gap: 0.9rem;
  margin: 0.5rem 0 1.2rem;
}

.cubesat-news-card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 92px;
  padding: 0.85rem 1rem;

  border: 1px solid #d0d7de !important;
  border-radius: 8px;

  background: #ffffff;
  color: inherit !important;

  box-shadow: none !important;
  background-image: none !important;
  text-decoration: none !important;

  transition:
    border-color 0.2s ease,
    transform 0.2s ease,
    box-shadow 0.2s ease;
}

.cubesat-news-card:hover,
.cubesat-news-card:focus,
.cubesat-news-card:active,
.cubesat-news-card:visited {
  text-decoration: none !important;
  background-image: none !important;
}

.cubesat-news-card:hover {
  border-color: #2486c7 !important;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.06) !important;
}

.cubesat-news-title {
  color: #2486c7;
  font-size: 0.88rem;
  font-weight: 700;
  line-height: 1.35;
}

.cubesat-news-meta {
  margin-top: 0.25rem;
  color: #6c757d;
  font-size: 0.72rem;
  font-weight: 500;
  line-height: 1.3;
}

/* =========================
   Divider
   ========================= */

.cubesat-section-divider {
  width: 100%;
  height: 1px;
  margin: 1.35rem 0 1.35rem;
  background: #d9dee3;
}

/* =========================
   Small project cards
   3 + 3 + 2 layout
   ========================= */

.cubesat-project-grid {
  display: grid;
  grid-template-columns: repeat(6, minmax(0, 1fr));
  gap: 0.75rem;
  width: 100%;
  max-width: 900px;
  margin: 0 auto 1.8rem;
}

.cubesat-project-card {
  grid-column: span 2;

  display: flex;
  flex-direction: column;
  justify-content: center;

  min-height: 76px;
  padding: 0.7rem 0.8rem;

  border: 1px solid #d0d7de;
  border-radius: 8px;

  background: #ffffff;

  transition:
    border-color 0.2s ease,
    transform 0.2s ease,
    box-shadow 0.2s ease;
}

/* Center the two cards in the final row. */
.cubesat-project-card:nth-last-child(2) {
  grid-column: 2 / span 2;
}

.cubesat-project-card:last-child {
  grid-column: 4 / span 2;
}

.cubesat-project-card:hover {
  border-color: #2486c7;
  transform: translateY(-2px);
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
}

.cubesat-project-title {
  color: #2486c7;
  font-size: 0.78rem;
  font-weight: 700;
  line-height: 1.3;
}

.cubesat-project-meta {
  margin-top: 0.22rem;
  color: #6c757d;
  font-size: 0.68rem;
  line-height: 1.3;
}

/* =========================
   CubeSat photo carousel
   ========================= */

.cubesat-carousel {
  position: relative;
  width: 100%;
  max-width: 850px;
  margin: 0 auto 1.5rem;
}

.cubesat-carousel-track {
  display: flex;
  width: 100%;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  scroll-behavior: smooth;
  -webkit-overflow-scrolling: touch;
  scrollbar-width: none;
  border-radius: 10px;
}

.cubesat-carousel-track::-webkit-scrollbar {
  display: none;
}

.cubesat-carousel-slide {
  flex: 0 0 100%;
  width: 100%;
  scroll-snap-align: start;
  scroll-snap-stop: always;
}

.cubesat-carousel-slide img {
  display: block;
  width: 100%;
  height: auto;
  margin: 0;
  border-radius: 10px;
  user-select: none;
  -webkit-user-drag: none;
}

.cubesat-carousel-arrow {
  position: absolute;
  top: calc(50% - 15px);
  transform: translateY(-50%);
  z-index: 10;

  display: flex;
  align-items: center;
  justify-content: center;

  width: 44px;
  height: 44px;
  padding: 0;

  border: none;
  border-radius: 50%;

  background: rgba(0, 0, 0, 0.5);
  color: #ffffff;

  font-size: 25px;
  line-height: 1;
  cursor: pointer;

  transition:
    background 0.2s ease,
    transform 0.2s ease,
    opacity 0.2s ease;
}

.cubesat-carousel-arrow:hover {
  background: rgba(0, 0, 0, 0.75);
}

.cubesat-carousel-arrow:active {
  transform: translateY(-50%) scale(0.94);
}

.cubesat-carousel-prev {
  left: 14px;
}

.cubesat-carousel-next {
  right: 14px;
}

.cubesat-carousel-dots {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 8px;
  margin-top: 12px;
}

.cubesat-carousel-dot {
  width: 9px;
  height: 9px;
  padding: 0;
  margin: 0;

  border: none;
  border-radius: 50%;

  background: #b9b9b9;
  cursor: pointer;

  transition:
    background 0.2s ease,
    transform 0.2s ease;
}

.cubesat-carousel-dot:hover {
  background: #777;
}

.cubesat-carousel-dot.active {
  background: #333;
  transform: scale(1.2);
}

/* =========================
   Responsive layout
   ========================= */

@media (max-width: 800px) {
  .cubesat-project-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .cubesat-project-card,
  .cubesat-project-card:nth-last-child(2),
  .cubesat-project-card:last-child {
    grid-column: auto;
  }
}

@media (max-width: 650px) {
  .cubesat-news-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 600px) {
  .cubesat-project-grid {
    grid-template-columns: 1fr;
  }

  .cubesat-carousel-arrow {
    width: 38px;
    height: 38px;
    font-size: 21px;
  }

  .cubesat-carousel-prev {
    left: 8px;
  }

  .cubesat-carousel-next {
    right: 8px;
  }
}

/* =========================
   Model screenshots
   ========================= */

.cubesat-model {
  margin: 1.5rem 0 2rem;
}

.cubesat-model-image {
  display: block;
  border: 1px solid var(--global-border-color, #d0d7de);
  border-radius: 8px;
  background: #fff;
}

.cubesat-model-image:focus-visible {
  outline: 3px solid #2486c7;
  outline-offset: 4px;
}

.cubesat-model-image img {
  display: block;
  width: 100%;
  height: auto;
  margin: 0;
  border-radius: 8px;
}

.cubesat-model figcaption {
  margin-top: 0.65rem;
  font-size: 0.9rem;
  line-height: 1.6;
  text-align: left;
}

.cubesat-model figcaption strong {
  display: block;
  color: var(--global-text-color, #333);
}

.cubesat-model-link {
  display: inline-block;
  margin-top: 0.4rem;
}

.cubesat-sil {
  margin: 0 0 2rem;
  padding: 0.85rem 1rem;
  border: 1px solid var(--global-border-color, #d0d7de);
  border-radius: 8px;
}

.cubesat-sil summary {
  cursor: pointer;
  font-weight: 700;
  line-height: 1.5;
}

.cubesat-sil summary:focus-visible {
  outline: 3px solid #2486c7;
  outline-offset: 4px;
}

.cubesat-sil .cubesat-model {
  margin: 1rem 0 0;
}
</style>

This competition gave participating teams the freedom to define their own CubeSat missions and design the spacecraft around the resulting requirements. After evaluating several mission concepts, our team developed Cubisa, a 3U CubeSat intended to demonstrate technologies relevant to tether-based space-debris removal and de-orbit maneuvering using dragsails.

The spacecraft consisted of the main satellite, named Q, and a detachable module, named Bisa, representing a target object. The proposed mission involved stabilizing the spacecraft after orbital injection, deploying Bisa using an inter-satellite tether, observing its relative motion through onboard imaging, retrieving and reconnecting it, reorienting the combined spacecraft, and finally deploying a drag sail to accelerate orbital decay.

Our design progressed through the conceptual and detailed design stages, placing us among the top four of 52 teams nationwide and securing funding to develop an engineering prototype. Our team ultimately finished in third place.

<div class="cubesat-news-grid">

  <a
    class="cubesat-news-card"
    href="https://www.citna.ir/news/337857/%D8%A8%D8%B1%DA%AF%D8%B2%D8%A7%D8%B1%DB%8C-%D9%85%D8%B1%D8%AD%D9%84%D9%87-%D8%A7%D8%B1%D8%B2%DB%8C%D8%A7%D8%A8%DB%8C-%D9%86%D9%87%D8%A7%DB%8C%DB%8C-%D8%B1%D9%88%DB%8C%D8%AF%D8%A7%D8%AF-%D9%81%D9%86%D8%A7%D9%88%D8%B1%D8%A7%D9%86%D9%87-%D8%B1%D9%82%D8%A7%D8%A8%D8%AA%DB%8C-%D8%B7%D8%B1%D8%A7%D8%AD%DB%8C-%D8%B3%D8%A7%D8%AE%D8%AA-%D9%85%D8%A7%D9%87%D9%88%D8%A7%D8%B1%D9%87-%D9%85%DA%A9%D8%B9%D8%A8%DB%8C-qsat"
    target="_blank"
    rel="noopener noreferrer">

    <span class="cubesat-news-title">
      Final phase announcement
    </span>

    <span class="cubesat-news-meta">
      Persian · External source ↗
    </span>

  </a>

  <a
    class="cubesat-news-card"
    href="https://snn.ir/fa/news/1191297/%D8%AD%D9%85%D8%A7%DB%8C%D8%AA-%DB%B6%DB%B0%DB%B0-%D9%85%DB%8C%D9%84%DB%8C%D9%88%D9%86-%D8%AA%D9%88%D9%85%D8%A7%D9%86%DB%8C-%D8%A7%D8%B2-%D8%AA%DB%8C%D9%85%E2%80%8C%D9%87%D8%A7%DB%8C-%D8%A8%D8%B1%D8%AA%D8%B1-%D8%B1%D9%88%DB%8C%D8%AF%D8%A7%D8%AF-%D9%81%D9%86%D8%A7%D9%88%D8%B1%D8%A7%D9%86%D9%87-qsat"
    target="_blank"
    rel="noopener noreferrer">

    <span class="cubesat-news-title">
      Detailed Design phase announcement
    </span>

    <span class="cubesat-news-meta">
      Persian · External source ↗
    </span>

  </a>

</div>

<div class="cubesat-section-divider"></div>

<div class="cubesat-project-grid">

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      Orbital Model
    </span>
    <span class="cubesat-project-meta">
      Simulation / Dynamics
    </span>
  </div>

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      SIL Testing
    </span>
    <span class="cubesat-project-meta">
      Validation / Control
    </span>
  </div>

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      PIL Testing
    </span>
    <span class="cubesat-project-meta">
      Embedded implementation
    </span>
  </div>

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      Detumbling
    </span>
    <span class="cubesat-project-meta">
      B-dot control
    </span>
  </div>

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      Nadir Pointing
    </span>
    <span class="cubesat-project-meta">
      Quaternion PD control
    </span>
  </div>

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      Sensor Fusion
    </span>
    <span class="cubesat-project-meta">
      Gyro / magnetometer / sun sensor
    </span>
  </div>

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      Magnetorquer Module
    </span>
    <span class="cubesat-project-meta">
      Actuation hardware
    </span>
  </div>

  <div class="cubesat-project-card">
    <span class="cubesat-project-title">
      Day/Night Logic
    </span>
    <span class="cubesat-project-meta">
      Sensor switching
    </span>
  </div>

</div>

<div class="cubesat-carousel">

  <button
    class="cubesat-carousel-arrow cubesat-carousel-prev"
    type="button"
    aria-label="Previous photo">
    &#10094;
  </button>

  <div class="cubesat-carousel-track">

    <div class="cubesat-carousel-slide">
      <img
        src="{{ '/images/cubesat-team.jpg' | relative_url }}"
        alt="Cubisa team during the national QSat competition"
        loading="eager"
        decoding="async">
    </div>

    <div class="cubesat-carousel-slide">
      <img
        src="{{ '/images/meeting.jpg' | relative_url }}"
        alt="Cubisa team during the CubeSat project"
        loading="lazy"
        decoding="async">
    </div>

    <div class="cubesat-carousel-slide">
      <img
        src="{{ '/images/magnetorquer.jpg' | relative_url }}"
        alt="Cubisa engineering prototype"
        loading="lazy"
        decoding="async">
    </div>

  </div>

  <button
    class="cubesat-carousel-arrow cubesat-carousel-next"
    type="button"
    aria-label="Next photo">
    &#10095;
  </button>

  <div class="cubesat-carousel-dots" aria-label="Photo navigation">

    <button
      class="cubesat-carousel-dot active"
      type="button"
      data-slide="0"
      aria-label="Show photo 1">
    </button>

    <button
      class="cubesat-carousel-dot"
      type="button"
      data-slide="1"
      aria-label="Show photo 2">
    </button>

    <button
      class="cubesat-carousel-dot"
      type="button"
      data-slide="2"
      aria-label="Show photo 3">
    </button>

  </div>

</div>

My role as a member of the Attitude Determination and Control System team involved translating the mission profile into ADCS requirements, researching, selecting and implementing the control architecture, developing the orbital and attitude dynamics simulation, defining reference frames and coordinate transformations, implementing and tuning the attitude controller, designing orbital day/night sensor-selection logic, combining sensor measurements to reduce noise and drift, and validating the system through software-in-the-loop and processor-in-the-loop testing.

<figure class="cubesat-model">
  <div class="cubesat-model-image">
    <img
      src="{{ '/images/Orbital_Model.jpg' | relative_url }}"
      alt="Simulink orbital model showing the propagator, atmospheric drag, Sun and eclipse models, geomagnetic field, and reference-frame transformations"
      width="2048"
      height="885"
      loading="lazy"
      decoding="async">
  </div>

  <figcaption>
    <strong>Orbital Model</strong>
  </figcaption>
</figure>

<figure class="cubesat-model">
  <div class="cubesat-model-image">
    <img
      src="{{ '/images/SIL.jpg' | relative_url }}"
      alt="Full Simulink SIL model showing the feedback connections between attitude commands, control, magnetic actuation, attitude dynamics, quaternion propagation, and sensor fusion"
      width="2048"
      height="1384"
      loading="lazy"
      decoding="async">
  </div>

  <figcaption>
    <strong>Software-in-the-Loop testing</strong>
  </figcaption>
</figure>

Although the circumstances in the country slowed down our progress repeatedly and caused HIL testing to remain unfinished, this project gave me practical experience with the development process of a CubeSat's control subsystem, from interpreting mission requirements and studying algorithms to mathematical modelling, sensor management, controller tuning, simulation, and embedded integration.

More importantly, it taught me that developing a control system is not only a matter of implementing equations from a paper. Every theoretical decision must remain consistent with the CubeSat's mission, coordinate conventions, sensor usage, actuator constraints, limitations of computational hardware, and validation strategy.

<script>
document.addEventListener("DOMContentLoaded", function () {
  document.querySelectorAll(".cubesat-carousel").forEach(function (carousel) {

    const track = carousel.querySelector(".cubesat-carousel-track");

    const slides = Array.from(
      carousel.querySelectorAll(".cubesat-carousel-slide")
    );

    const dots = Array.from(
      carousel.querySelectorAll(".cubesat-carousel-dot")
    );

    const previousButton = carousel.querySelector(
      ".cubesat-carousel-prev"
    );

    const nextButton = carousel.querySelector(
      ".cubesat-carousel-next"
    );

    let currentSlide = 0;

    function updateDots(index) {
      dots.forEach(function (dot, dotIndex) {
        dot.classList.toggle("active", dotIndex === index);
      });
    }

    function goToSlide(index) {

      if (index < 0) {
        index = slides.length - 1;
      }

      if (index >= slides.length) {
        index = 0;
      }

      currentSlide = index;

      track.scrollTo({
        left: track.clientWidth * currentSlide,
        behavior: "smooth"
      });

      updateDots(currentSlide);
    }

    previousButton.addEventListener("click", function () {
      goToSlide(currentSlide - 1);
    });

    nextButton.addEventListener("click", function () {
      goToSlide(currentSlide + 1);
    });

    dots.forEach(function (dot, index) {
      dot.addEventListener("click", function () {
        goToSlide(index);
      });
    });

    let scrollTimer;

    track.addEventListener("scroll", function () {

      clearTimeout(scrollTimer);

      scrollTimer = setTimeout(function () {

        const index = Math.round(
          track.scrollLeft / track.clientWidth
        );

        currentSlide = Math.max(
          0,
          Math.min(index, slides.length - 1)
        );

        updateDots(currentSlide);

      }, 60);
    });

    window.addEventListener("resize", function () {
      track.scrollLeft = track.clientWidth * currentSlide;
    });

  });
});
</script>
