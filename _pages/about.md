---
layout: page
title: Home
permalink: /
nav: false
nav_order: 1
---

<style>
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

  .hsp-lede {
    margin-bottom: 2rem;
  }

  .hsp-lede p {
    margin: 0 0 0.65rem;
  }

  .hsp-lede p:last-child {
    margin-bottom: 0;
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
  }

  .hsp-people {
    display: grid;
    gap: 1.5rem 1.25rem;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    margin: 1.5rem 0 2rem;
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
</style>

<h1 class="hsp-page-title">40th Annual Conference on Human Sentence Processing</h1>

<div class="hsp-lede">
  <p><strong>Dates:</strong> May 20-22, 2027</p>
  <p><strong>Location:</strong> Purdue University, West Lafayette, Indiana</p>
  <p><strong>Special theme:</strong> Cognitive Mechanisms of Syntactic Change Throughout the Lifespan</p>
</div>

## Invited Speakers

<div class="hsp-people">
  {% for person in site.data.speakers %}
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

Please contact us at hsp2027@gmail.com with any questions about the conference.
Check [HSP Society](https://www.hspsociety.org/home) for more information, and subscribe to the HSP mailing list [here](https://www.hspsociety.org/get-involved).
