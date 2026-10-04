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
    font-size: clamp(1.75rem, 2.6vw, 2.25rem);
    font-weight: 700;
    line-height: 1.12;
    margin-bottom: 1.75rem;
    max-width: 100%;
    text-align: center;
    white-space: nowrap;
  }

  .hsp-event-details {
    border-bottom: 1px solid var(--global-divider-color);
    border-top: 1px solid var(--global-divider-color);
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    margin: 0 0 3rem;
  }

  .hsp-event-detail {
    padding: 1.1rem 1.25rem;
  }

  .hsp-event-detail + .hsp-event-detail {
    border-left: 1px solid var(--global-divider-color);
  }

  .hsp-event-label {
    color: var(--global-text-color-light);
    display: block;
    font-size: 0.9rem;
    font-weight: 700;
    margin-bottom: 0.35rem;
  }

  .hsp-event-value {
    font-size: 1.08rem;
    line-height: 1.45;
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

    .hsp-event-details {
      grid-template-columns: 1fr;
    }

    .hsp-event-detail + .hsp-event-detail {
      border-left: 0;
      border-top: 1px solid var(--global-divider-color);
    }
  }

  .hsp-people {
    display: grid;
    gap: 1.5rem 1.25rem;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    margin: 1.5rem 0 2rem;
  }

  .hsp-speakers {
    display: grid;
    gap: 0 2rem;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    margin: 1.5rem 0 2rem;
  }

  .hsp-speaker {
    align-items: center;
    border-top: 1px solid var(--global-divider-color);
    display: grid;
    gap: 1rem;
    grid-template-columns: 148px minmax(0, 1fr);
    padding: 1.25rem 0;
  }

  .hsp-speaker:nth-child(-n + 2) {
    border-top: 0;
  }

  .hsp-speaker img {
    aspect-ratio: 1 / 1;
    border: 1px solid var(--global-divider-color);
    border-radius: 50%;
    height: 148px;
    object-fit: cover;
    width: 148px;
  }

  .hsp-speaker-name {
    color: var(--global-text-color);
    display: inline-block;
    font-size: 1.15rem;
    font-weight: 700;
    line-height: 1.25;
    margin-bottom: 0.35rem;
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
    height: 120px;
    object-fit: cover;
    width: 120px;
  }

  .hsp-person strong {
    display: block;
    font-size: 0.98rem;
    margin-top: 0.65rem;
  }

  .hsp-person span {
    color: var(--global-text-color-light);
    display: block;
    font-size: 0.9rem;
    line-height: 1.35;
  }

  @media (max-width: 900px) {
    .hsp-speakers {
      grid-template-columns: 1fr;
    }

    .hsp-speaker:nth-child(-n + 2) {
      border-top: 1px solid var(--global-divider-color);
    }

    .hsp-speaker:first-child {
      border-top: 0;
    }
  }
</style>

<h1 class="hsp-page-title">40th Annual Conference on Human Sentence Processing</h1>

<div class="hsp-event-details">
  <div class="hsp-event-detail">
    <span class="hsp-event-label">Dates</span>
    <div class="hsp-event-value">May 20-22, 2027</div>
  </div>
  <div class="hsp-event-detail">
    <span class="hsp-event-label">Location</span>
    <div class="hsp-event-value">Purdue University, West Lafayette, Indiana</div>
  </div>
</div>

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

## Organizing Committee

<div class="hsp-people">
  {% for person in site.data.committee %}
    <div class="hsp-person">
      <a href="{{ person.url }}" target="_blank" rel="noopener">
        <img
          src="{{ person.photo | relative_url }}"
          alt="{{ person.name }}"
          onerror="this.onerror=null;this.src='{{ '/assets/img/committee/placeholder.svg' | relative_url }}';"
        >
        <strong>{{ person.name }}</strong>
      </a>
      <span>{{ person.affiliation }}</span>
    </div>
  {% endfor %}
</div>

## Important Dates

- [Reviewer sign-up](https://docs.google.com/forms/d/e/1FAIpQLSd7m42hCJ7IXNn49TUO32HfoOCHiLx25Yi1TWes2UYvxns5nA/viewform) deadline: December 15, 2026
- [Abstract submission](https://oxfordabstracts.com/) deadline: January 15, 2027
- Notification of acceptance: TBA
- [Early registration](https://www.hspsociety.org/home) deadline: TBA
- [Conference registration](https://www.hspsociety.org/home) deadline: TBA
- Travel grants application deadline: TBA
- Conference dates: May 20-22, 2027

## Contact

For questions about **HSP 2027**, please contact the organizing committee at [hsp2027@gmail.com](mailto:hsp2027@gmail.com).

### Accessibility

HSP 2027 is committed to making the conference accessible to all participants. If you have accessibility requirements or would like to discuss accommodations, please contact the organizing committee at [hsp2027@gmail.com](mailto:hsp2027@gmail.com) as early as possible.

For general information about the Human Sentence Processing Society, visit the [HSP Society website](https://www.hspsociety.org/home). To receive HSP announcements, subscribe to the [HSP mailing list](https://www.hspsociety.org/get-involved).
