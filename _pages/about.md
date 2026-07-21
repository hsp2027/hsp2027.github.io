---
layout: page
title: 40th Annual Conference on Human Sentence Processing
permalink: /
nav: false
nav_order: 1
---

<style>
  .hsp-lede {
    margin-bottom: 2rem;
  }

  .hsp-meta {
    margin: 1.25rem 0 1.75rem;
    padding-left: 1.1rem;
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

<div class="hsp-lede">
  <p><strong>Dates:</strong> May 20-22, 2027</p>
  <p><strong>Location:</strong> Purdue University, West Lafayette, Indiana</p>
</div>

**Special theme:** Cognitive mechanisms of syntactic change throughout the lifespan

Examining a variety of perspectives on how and why syntactic representations develop and change in individuals due to age-related cognitive development (children and adults), changes in input characteristics (e.g. through moving to a new multilingual context or new dialect region), or changes due to experiment participation, classroom language teaching, or clinical interventions.

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
      <span>{{ person.title }}, {{ person.affiliation }}</span>
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

## Contact

Please contact us at hsp2027@gmail.com with any questions regarding the conference. Let us know what we can do to make the conference accessible to you.
