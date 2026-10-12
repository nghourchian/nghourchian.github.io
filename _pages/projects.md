---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: false
---

<style>
.archive {
  float: none !important;
  width: 100% !important;
  padding-left: 0 !important;
  margin-left: auto !important;
  margin-right: auto !important;
}

.archive .page__title {
  width: 100%;
  max-width: 1250px;
  margin-left: auto;
  margin-right: auto;
}

/* Featured projects */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 460px));
  justify-content: center;
  column-gap: clamp(3rem, 9vw, 14rem);
  row-gap: 2.4rem;
  width: 100%;
  max-width: 1250px;
  margin: 1.5rem auto 0;
}

.project-card {
  display: flex;
  flex-direction: column;
  min-width: 0;
  background: #ffffff;
  border: 1px solid #eeeeee;
  border-radius: 14px;
  overflow: hidden;
  box-shadow: 0 8px 28px rgba(0, 0, 0, 0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 14px 34px rgba(0, 0, 0, 0.13);
}

.project-card > a {
  display: block;
}

.project-image-wrapper {
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 9;
  overflow: hidden;
}

.project-image-wrapper img,
.project-image-wrapper video {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.project-year-badge {
  position: absolute;
  top: 0;
  right: 0;
  padding: 0.6rem 0.8rem;
  border-bottom-left-radius: 14px;
  background: #222222;
  color: #ffffff;
  font-size: 0.78rem;
  font-weight: 700;
  white-space: nowrap;
}

.project-content {
  display: flex;
  flex-direction: column;
  flex: 1;
  padding: 1.2rem;
}

.project-title {
  margin-top: 0;
  margin-bottom: 0.9rem;
  font-size: 1.25rem;
  line-height: 1.35;
  font-weight: 700;
}

.project-title a {
  color: #24364a;
  text-decoration: none;
}

.project-title a:hover {
  color: #4f68e8;
}

.project-meta {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  padding: 0.7rem 0.85rem;
  margin-bottom: 1.1rem;
  border-left: 4px solid #6177f2;
  border-radius: 8px;
  background: #f7f8fb;
  color: #344054;
  font-size: 0.85rem;
  font-weight: 600;
}

.project-meta span {
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  min-width: 0;
}

.drone-icon {
  width: 1.4em;
  height: 1.4em;
  object-fit: contain;
  flex-shrink: 0;
}

.project-button {
  display: b;
  margin-top: auto;
  padding: 0.75rem 1rem;
  border-radius: 8px;
  background: #6177f2;
  color: #ffffff !important;
  text-align: center;
  text-decoration: none !important;
  font-weight: 700;
  transition: background 0.2s ease;
}

.project-button:hover {
  background: #4f63dc;
}

.project-button,
.project-button:link,
.project-button:visited,
.project-button:hover,
.project-button:focus,
.project-button:active {
  text-decoration: none !important;
  border-bottom: none !important;
  box-shadow: none !important;
  background-image: none !important;
}

/* Divider */
.projects-divider {
  width: 100%;
  max-width: 1250px;
  height: 1px;
  margin: 2.5rem auto 2rem;
  background: #d9dee3;
}

/* Smaller projects */
.small-projects-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.2rem;
  width: 100%;
  max-width: 1150px;
  margin: 0 auto 3rem;
}

.small-project-card {
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-width: 0;
  min-height: 135px;
  padding: 1.15rem 1.2rem;
  background: #ffffff;
  border: 1px solid #e4e7ec;
  border-radius: 12px;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.045);
  transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
}

.small-project-card:hover {
  transform: translateY(-4px);
  border-color: #c8cff9;
  box-shadow: 0 8px 22px rgba(0, 0, 0, 0.08);
}

.small-project-title {
  margin: 0 0 0.45rem;
  color: #24364a;
  font-size: 1rem;
  font-weight: 700;
  line-height: 1.35;
}

.small-project-type {
  margin: 0;
  color: #667085;
  font-size: 0.8rem;
  font-weight: 500;
  line-height: 1.4;
}

/* Cards with images */
.small-project-card--linked,
.small-project-card--static {
  flex-direction: row;
  align-items: center;
  justify-content: flex-start;
  gap: 0.85rem;
  padding: 0.75rem;
  text-decoration: none !important;
  color: inherit;
}

.small-project-card--linked:hover,
.small-project-card--linked:focus {
  text-decoration: none !important;
}

.small-project-card--linked:hover .small-project-title {
  color: #4f68e8;
}

.small-project-card--linked:focus-visible {
  outline: 2px solid #6177f2;
  outline-offset: 3px;
}

.small-project-card--static:hover {
  transform: none;
  border-color: #e4e7ec;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.045);
}

.small-project-details {
  flex: 1;
  min-width: 0;
}

.small-project-image {
  display: b;
  flex: 0 0 42%;
  width: 42%;
  height: 110px;
  object-fit: contain;
  border-radius: 8px;
  background: #f7f8fb;
}

/* H-bridge image pair */
.hbridge-collage {
  position: relative;
  flex: 0 0 44%;
  width: 44%;
  height: 120px;
}

.hbridge-collage img {
  position: absolute;
  display: b;
  width: 70%;
  height: 78px;
  object-fit: contain;
  border: 1px solid #e4e7ec;
  border-radius: 8px;
  background: #f7f8fb;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.08);
}

.hbridge-proteus {
  top: 0;
  right: 0;
  z-index: 2;
}

.hbridge-hardware {
  bottom: 0;
  left: 0;
  z-index: 1;
}

/* Responsive design */
@media (max-width: 900px) {
  .projects-grid {
    grid-template-columns: minmax(0, 1fr);
    max-width: 540px;
    row-gap: 1.8rem;
  }

  .small-projects-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    max-width: 700px;
  }
}

@media (max-width: 600px) {
  .small-projects-grid {
    grid-template-columns: minmax(0, 1fr);
  }

  .project-content {
    padding: 1rem;
  }

  .project-title {
    font-size: 1.15rem;
  }

  .project-year-badge {
    padding: 0.5rem 0.65rem;
    font-size: 0.72rem;
  }

  .small-project-card {
    min-height: 110px;
    padding: 1rem 1.1rem;
  }

  .small-project-card--linked,
  .small-project-card--static {
    padding: 0.75rem;
  }
}
</style>

<!-- Featured projects -->
<div class="projects-grid">

  <div class="project-card">
    <a href="/projects/cubesat-adcs/">
      <div class="project-image-wrapper">
        <img src="/images/cubesat-team.jpg" alt="3U CubeSat ADCS team">
        <div class="project-year-badge">Jan 2024 — Jul 2026</div>
      </div>
    </a>

    <div class="project-content">
      <h2 class="project-title">
        <a href="/projects/cubesat-adcs/">Attitude Determination and Control System</a>
      </h2>
      <div class="project-meta">
        <span>🛰 National CubeSat Design Competition (Qsat)</span>
      </div>
      <a class="project-button" href="/projects/cubesat-adcs/">Project Details</a>
    </div>
  </div>

  <div class="project-card">
    <a href="/projects/gps-denied-navigation/">
      <div class="project-image-wrapper">
        <video autoplay muted loop playsinline preload="metadata">
          <source src="/videos/gps-denied-navigation.mp4" type="video/mp4">
        </video>
        <div class="project-year-badge">Jun 2025 — Jan 2026</div>
      </div>
    </a>

    <div class="project-content">
      <h2 class="project-title">
        <a href="/projects/gps-denied-navigation/">Vision-Based GPS-Denied Navigation for Emergency Response UAVs</a>
      </h2>
      <div class="project-meta">
        <span>
          <img src="/images/drone-icon.png" alt="" class="drone-icon">
          Bachelor’s Final Project
        </span>
      </div>
      <a class="project-button" href="/projects/gps-denied-navigation/">Project Details</a>
    </div>
  </div>

</div>

<div class="projects-divider"></div>

<!-- Smaller projects -->
<div class="small-projects-grid">

  <a class="small-project-card small-project-card--linked"
     href="https://github.com/nghourchian/h-bridge-dc-motor-driver"
     target="_blank"
     rel="noopener noreferrer"
     aria-label="View H-Bridge DC Motor Driver Design on GitHub">

    <div class="hbridge-collage">
      <img class="hbridge-proteus"
           src="https://raw.githubusercontent.com/nghourchian/h-bridge-dc-motor-driver/main/H-Bridge-DC-Motor-Driver.bmp"
           alt="Proteus H-bridge circuit schematic"
           loading="lazy">
      <img class="hbridge-hardware"
           src="https://raw.githubusercontent.com/nghourchian/h-bridge-dc-motor-driver/main/H-Bridge%20Breadboard.jpg"
           alt="H-bridge breadboard circuit photograph"
           loading="lazy">
    </div>

    <div class="small-project-details">
      <h3 class="small-project-title">H-Bridge DC Motor Driver Design</h3>
      <p class="small-project-type">Electronics</p>
    </div>
  </a>

  <a class="small-project-card small-project-card--linked"
     href="https://github.com/nghourchian/face-recognition-door-"
     target="_blank"
     rel="noopener noreferrer"
     aria-label="View Facial Detection Door  on GitHub">

    <img class="small-project-image"
         src="/images/face-.png"
         alt="Face recognition application with anti-spoofing scores and lock status"
         loading="lazy">

    <div class="small-project-details">
      <h3 class="small-project-title">Facial Detection Door Lock</h3>
      <p class="small-project-type">Computer Vision</p>
    </div>
  </a>

  <a class="small-project-card small-project-card--linked"
     href="https://github.com/nghourchian/reduction-gearbox-cad"
     target="_blank"
     rel="noopener noreferrer"
     aria-label="View Reduction Gearbox CAD Design on GitHub">

    <img class="small-project-image"
         src="https://raw.githubusercontent.com/nghourchian/reduction-gearbox-cad/main/Assembly.JPG"
         alt="Reduction gearbox CAD assembly"
         loading="lazy">

    <div class="small-project-details">
      <h3 class="small-project-title">Reduction Gearbox CAD Design</h3>
      <p class="small-project-type">Mechanical Design</p>
    </div>
  </a>

  <a class="small-project-card small-project-card--linked"
     href="https://github.com/nghourchian/temperature-control-system"
     target="_blank"
     rel="noopener noreferrer"
     aria-label="View Temperature Control System Design on GitHub">

    <img class="small-project-image"
         src="/images/temp-control.jpg"
         alt="Temperature control system project"
         loading="lazy">

    <div class="small-project-details">
      <h3 class="small-project-title">Temperature Control System Design</h3>
      <p class="small-project-type">Control Systems</p>
    </div>
  </a>



  <a class="small-project-card small-project-card--linked"
     href="https://github.com/nghourchian/target-tracking-and-capture"
     target="_blank"
     rel="noopener noreferrer"
     aria-label="View Target Tracking and Capture in ROS2 Turtlesim on GitHub">

    <img class="small-project-image"
         src="/images/turtlesim.jpg"
         alt="Target tracking and capture in ROS2 Turtlesim"
         loading="lazy">

    <div class="small-project-details">
      <h3 class="small-project-title">Target Tracking and Capture in ROS2 Turtlesim</h3>
      <p class="small-project-type">Robotics</p>
    </div>
  </a>

</div>
