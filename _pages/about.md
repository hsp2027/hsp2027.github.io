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
    font-size: clamp(2rem, 4vw, 3.25rem);
    font-weight: 700;
    line-height: 1.12;
    margin: 0;
    max-width: 100%;
    white-space: nowrap;
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
    font-size: 1.1rem;
    line-height: 1.45;
  }

  .hsp-event-label {
    font-weight: 700;
  }

  .hsp-theme-name {
    font-size: 1.2rem;
    font-style: italic;
    font-weight: 700;
    line-height: 1.45;
    margin: 0 0 0.85rem;
  }

  .hsp-theme-copy {
    font-size: 1.03rem;
    line-height: 1.65;
    margin: 0;
    max-width: 48rem;
  }

  h2 {
    font-size: 1.45rem;
    font-weight: 700;
    margin-top: 2.75rem;
    margin-bottom: 1rem;
  }

  @media (max-width: 900px) {
    .hsp-page-title {
      white-space: normal;
    }

    .hsp-hero {
      min-height: 28rem;
      padding: 1.5rem;
    }
  }

  .hsp-people {
    display: grid;
    gap: 1.5rem 1.25rem;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    margin: 1.5rem auto 2rem;
    max-width: 58rem;
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
    min-height: 21rem;
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
    font-size: 1.15rem;
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
    line-height: 1.4;
  }

  .hsp-speaker-affiliation {
    color: var(--global-text-color-light);
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

  .hsp-people .hsp-person:nth-last-child(2):nth-child(4n + 1) {
    grid-column: 2;
  }

  .hsp-person .hsp-person-role {
    color: var(--global-theme-color);
    display: block;
    font-size: 0.78rem;
    font-weight: 700;
    line-height: 1.35;
    margin-top: 0.25rem;
  }

  .hsp-dates {
    border-top: 1px solid var(--global-divider-color);
    margin: 1.25rem 0 0;
    max-width: 58rem;
  }

  .hsp-date-row {
    align-items: baseline;
    border-bottom: 1px solid var(--global-divider-color);
    display: grid;
    gap: 1rem;
    grid-template-columns: minmax(0, 1fr) auto;
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
    max-width: 58rem;
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

    .hsp-people .hsp-person:nth-last-child(2):nth-child(4n + 1) {
      grid-column: auto;
    }

    .hsp-date-row {
      gap: 0.2rem;
      grid-template-columns: 1fr;
    }

    .hsp-date-value {
      text-align: left;
    }
  }
</style>

<section class="hsp-hero" role="img" aria-label="Purdue University campus">
  <div class="hsp-hero-content">
    <h1 class="hsp-page-title">40th Annual Conference on Human Sentence Processing</h1>

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

<p class="hsp-theme-name">Cognitive Mechanisms of Syntactic Change Throughout the Lifespan</p>

<p class="hsp-theme-copy">Examining a variety of perspectives on how and why syntactic representations develop and change throughout the lifespan. Relevant topics may include age-related cognitive development in children and adults, changes in linguistic input characteristics (e.g. adapting to a new multilingual context), and changes resulting from experiment participation, written language exposure, classroom instruction, or clinical interventions.</p>

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

## Organizing Team

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

## Important Dates

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

## Contact

For questions about **HSP 2027**, please contact the organizing committee at [hsp2027@gmail.com](mailto:hsp2027@gmail.com).

### Accessibility

HSP 2027 is committed to making the conference accessible to all participants. If you have accessibility requirements or would like to discuss accommodations, please contact the organizing committee at [hsp2027@gmail.com](mailto:hsp2027@gmail.com) as early as possible.

For general information about the Human Sentence Processing Society, visit the [HSP Society website](https://www.hspsociety.org/home). To receive HSP announcements, subscribe to the [HSP mailing list](https://www.hspsociety.org/get-involved).
