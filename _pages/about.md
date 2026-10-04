---
layout: page
title: Home
permalink: /
nav: false
nav_order: 1
---

<style>
  :root {
    --global-theme-color: #8e6f3e;
    --global-hover-color: #8e6f3e;
    --global-code-bg-color: rgba(142, 111, 62, 0.08);
  }

  html[data-theme="dark"] {
    --global-theme-color: #cfb991;
    --global-hover-color: #cfb991;
    --global-code-bg-color: rgba(207, 185, 145, 0.12);
  }

  .post-header {
    display: none;
  }

  .hsp-page-title {
    color: #fff;
    font-size: clamp(1.9rem, 3.25vw, 2.65rem);
    font-weight: 700;
    line-height: 1.12;
    margin: 0;
    max-width: 100%;
    white-space: normal;
  }

  .hsp-hero {
    background-image: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url("https://www.purdue.edu/newsroom/wp-content/uploads/2025/10/THE-GUV26.jpg");
    background-position: center;
    background-size: cover;
    color: #fff;
    display: flex;
    min-height: 25rem;
    padding: 2.5rem;
  }

  .hsp-hero-content {
    align-self: flex-end;
    max-width: 54rem;
  }

  .hsp-event-details {
    display: flex;
    flex-direction: column;
    gap: 0.45rem;
    margin-top: 1.5rem;
  }

  .hsp-event-detail {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
  }

  .hsp-event-label,
  .hsp-event-value {
    color: #fff;
    font-size: 1.1rem;
    line-height: 1.45;
  }

  .hsp-event-label {
    font-weight: 700;
  }

  .hsp-theme-name {
    font-size: 1.2rem;
    font-weight: 700;
    line-height: 1.45;
    margin: 0 0 0.85rem;
  }

  .hsp-theme-feature {
    background: color-mix(in srgb, var(--global-theme-color) 5%, transparent);
    border-left: 4px solid var(--global-theme-color);
    margin-top: 1rem;
    padding: 1.25rem 1.5rem;
  }

  .hsp-theme-copy {
    font-size: 1.03rem;
    line-height: 1.65;
    margin: 0;
  }

  h2 {
    font-size: 1.45rem;
    font-weight: 700;
    margin-top: 2.75rem;
    margin-bottom: 1rem;
  }

  @media (max-width: 900px) {
    .hsp-hero {
      min-height: 28rem;
      padding: 1.5rem;
    }
  }

  .hsp-people {
    display: grid;
    gap: 1.5rem 1.25rem;
    grid-template-columns: repeat(5, minmax(0, 1fr));
    margin: 1.5rem 0 2rem;
  }

  .hsp-speakers {
    display: grid;
    gap: 1.25rem;
    grid-template-columns: repeat(6, minmax(0, 1fr));
    margin: 1.5rem 0 2rem;
  }

  .hsp-speaker {
    align-items: center;
    background: color-mix(in srgb, var(--global-theme-color) 5%, transparent);
    border: 1px solid var(--global-divider-color);
    border-radius: 6px;
    display: flex;
    flex-direction: column;
    grid-column: span 2;
    min-height: 18rem;
    padding: 1.35rem;
    text-align: center;
  }

  .hsp-speaker:nth-last-child(2):nth-child(3n + 1) {
    grid-column: 2 / span 2;
  }

  .hsp-speaker img {
    aspect-ratio: 1 / 1;
    border: 1px solid var(--global-divider-color);
    border-radius: 50%;
    height: 152px;
    object-fit: cover;
    width: 152px;
  }

  .hsp-speaker-name {
    color: var(--global-text-color);
    display: inline-block;
    font-size: 1.05rem;
    font-weight: 700;
    line-height: 1.25;
    margin: 0.9rem 0 0.35rem;
  }

  .hsp-speaker-role,
  .hsp-speaker-affiliation,
  .hsp-speaker-talk {
    margin: 0;
  }

  .hsp-speaker-role {
    font-size: 0.93rem;
    line-height: 1.4;
  }

  .hsp-speaker-affiliation {
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    line-height: 1.4;
    margin-top: 0.2rem;
  }

  .hsp-speaker-talk {
    font-style: italic;
    line-height: 1.4;
    margin-top: 0.65rem;
  }

  .hsp-person {
    text-align: center;
  }

  .hsp-person img {
    aspect-ratio: 1 / 1;
    border: 1px solid var(--global-divider-color);
    border-radius: 50%;
    height: 96px;
    object-fit: cover;
    width: 96px;
  }

  .hsp-person strong {
    display: block;
    font-size: 0.9rem;
    margin-top: 0.5rem;
  }

  .hsp-person span {
    color: var(--global-text-color-light);
    display: block;
    font-size: 0.82rem;
    line-height: 1.35;
  }

  @media (max-width: 900px) {
    .hsp-speakers {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .hsp-speaker {
      grid-column: auto;
    }

    .hsp-speaker:nth-last-child(2):nth-child(3n + 1) {
      grid-column: auto;
    }

    .hsp-people {
      grid-template-columns: repeat(2, minmax(0, 1fr));
      max-width: 34rem;
    }
  }

  .hsp-person .hsp-person-role {
    color: var(--global-theme-color);
    display: block;
    font-size: 0.78rem;
    font-weight: 400;
    line-height: 1.35;
    margin-top: 0.25rem;
  }

  .hsp-dates {
    border-top: 1px solid var(--global-divider-color);
    margin: 1.25rem 0 0;
  }

  .hsp-date-row {
    align-items: baseline;
    border-bottom: 1px solid var(--global-divider-color);
    display: grid;
    gap: 1.25rem;
    grid-template-columns: minmax(0, 17rem) max-content;
    padding: 0.7rem 0;
  }

  .hsp-date-value {
    text-align: right;
    white-space: nowrap;
  }

  .hsp-date-note {
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    line-height: 1.45;
    margin: 0.85rem 0 0;
  }

  .hsp-info-panels {
    display: grid;
    gap: 1.25rem;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    margin: 2.75rem 0;
  }

  .hsp-info-panel {
    background: color-mix(in srgb, var(--global-theme-color) 5%, transparent);
    border: 1px solid var(--global-divider-color);
    border-radius: 6px;
    padding: 1.5rem;
  }

  .hsp-info-panel h2 {
    font-size: 1.45rem;
    margin: 0;
  }

  .hsp-info-panel h3 {
    font-size: 1rem;
    font-weight: 700;
    margin: 1.35rem 0 0.35rem;
  }

  .hsp-info-panel p {
    margin: 0;
  }

  @media (max-width: 600px) {
    .hsp-speakers,
    .hsp-people {
      grid-template-columns: 1fr;
    }

    .hsp-speaker {
      min-height: 0;
    }

    .hsp-people {
      max-width: 16rem;
    }

    .hsp-date-row {
      gap: 0.2rem;
      grid-template-columns: 1fr;
    }

    .hsp-date-value {
      text-align: left;
    }

    .hsp-info-panels {
      grid-template-columns: 1fr;
    }
  }
</style>

<section class="hsp-hero" role="img" aria-label="Purdue University campus">
  <div class="hsp-hero-content">
    <h1 class="hsp-page-title">40th Annual Conference on Human Sentence Processing (HSP 2027)</h1>

    <div class="hsp-event-details">
      <div class="hsp-event-detail">
        <span class="hsp-event-label">Dates:</span>
        <span class="hsp-event-value">May 20-22, 2027</span>
      </div>
      <div class="hsp-event-detail">
        <span class="hsp-event-label">Location:</span>
        <span class="hsp-event-value">Purdue University, West Lafayette, Indiana</span>
      </div>
    </div>
  </div>
</section>

## Special Theme

<div class="hsp-theme-feature">
  <p class="hsp-theme-name">Cognitive Mechanisms of Syntactic Change Throughout the Lifespan</p>
  <p class="hsp-theme-copy">Examining a variety of perspectives on how and why syntactic representations develop and change throughout the lifespan. Relevant topics may include age-related cognitive development in children and adults, changes in linguistic input characteristics (e.g. adapting to a new multilingual context), and changes resulting from experiment participation, written language exposure, classroom instruction, or clinical interventions.</p>
</div>

## Invited Speakers

<div class="hsp-speakers">
  {% for person in site.data.speakers %}
    <div class="hsp-speaker">
      <a href="{{ person.url }}" target="_blank" rel="noopener">
        <img
          src="{{ person.photo | relative_url }}"
          alt="{{ person.name }}"
          onerror="this.onerror=null;this.src='{{ '/assets/img/committee/placeholder.svg' | relative_url }}';"
        >
      </a>
      <div>
        <a class="hsp-speaker-name" href="{{ person.url }}" target="_blank" rel="noopener">{{ person.name }}</a>
        <p class="hsp-speaker-role">{{ person.title }}</p>
        <p class="hsp-speaker-affiliation">{{ person.affiliation }}</p>
        {% if person.talk_title %}
          <p class="hsp-speaker-talk">Talk: {{ person.talk_title }}</p>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>

## Organizing Committee

<div class="hsp-people">
  {% for person in site.data.committee %}
    <div class="hsp-person">
      <a href="{{ person.url }}" target="_blank" rel="noopener">
        <img
          src="{% if person.photo_url %}{{ person.photo_url }}{% else %}{{ person.photo | relative_url }}{% endif %}"
          alt="{{ person.name }}"
          onerror="this.onerror=null;this.src='{{ '/assets/img/committee/placeholder.svg' | relative_url }}';"
        >
        <strong>{{ person.name }}</strong>
      </a>
      <span>{{ person.affiliation }}</span>
      {% if person.role %}
        <span class="hsp-person-role">{{ person.role }}</span>
      {% endif %}
    </div>
  {% endfor %}
</div>

<div class="hsp-info-panels">
  <section class="hsp-info-panel">
    <h2>Important Dates</h2>
    <div class="hsp-dates">
      <div class="hsp-date-row">
        <span><a href="https://docs.google.com/forms/d/e/1FAIpQLSd7m42hCJ7IXNn49TUO32HfoOCHiLx25Yi1TWes2UYvxns5nA/viewform">Reviewer sign-up deadline</a></span>
        <span class="hsp-date-value">December 15, 2026</span>
      </div>
      <div class="hsp-date-row">
        <span><a href="https://oxfordabstracts.com/">Abstract submission deadline</a></span>
        <span class="hsp-date-value">January 15, 2027</span>
      </div>
      <div class="hsp-date-row">
        <span>Notification of acceptance</span>
        <span class="hsp-date-value">TBA</span>
      </div>
      <div class="hsp-date-row">
        <span><a href="https://www.hspsociety.org/home">Early registration deadline</a></span>
        <span class="hsp-date-value">TBA</span>
      </div>
      <div class="hsp-date-row">
        <span><a href="https://www.hspsociety.org/home">Conference registration deadline</a></span>
        <span class="hsp-date-value">TBA</span>
      </div>
      <div class="hsp-date-row">
        <span>Travel grants application deadline</span>
        <span class="hsp-date-value">TBA</span>
      </div>
      <div class="hsp-date-row">
        <span>Conference dates</span>
        <span class="hsp-date-value">May 20-22, 2027</span>
      </div>
    </div>
    <p class="hsp-date-note">All submission and application deadlines are at 11:59 p.m. UTC-12 (Anywhere on Earth, AoE), unless otherwise noted.</p>
  </section>

  <section class="hsp-info-panel">
    <h2>Get in Touch</h2>
    <h3>Questions about HSP 2027?</h3>
    <p>Please email us at <a href="mailto:hsp2027@gmail.com">hsp2027@gmail.com</a>.</p>

    <h3>Accessibility and Accommodations</h3>
    <p>HSP 2027 is committed to making the conference accessible to all participants. If you have specific accessibility needs or would like to discuss accommodations, please contact us at <a href="mailto:hsp2027@gmail.com">hsp2027@gmail.com</a> as early as possible.</p>

    <h3>HSP Community</h3>
    <p>For general information about the Human Sentence Processing Society, visit the <a href="https://www.hspsociety.org/home">HSP Society website</a>.</p>
    <p>To receive announcements, subscribe to the <a href="https://www.hspsociety.org/get-involved">HSP mailing list</a>.</p>
  </section>
</div>
