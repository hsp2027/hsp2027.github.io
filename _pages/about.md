---
layout: page
title: Home
permalink: /
nav: true
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

# HSP 2027

<div class="hsp-lede">
  <p><strong>40th Annual Conference on Human Sentence Processing</strong></p>
  <ul class="hsp-meta">
    <li><strong>Host:</strong> Purdue University, West Lafayette, Indiana</li>
    <li><strong>Dates:</strong> May 20-22, 2027</li>
    <li><strong>Special theme:</strong> Cognitive mechanisms of syntactic change throughout the lifespan</li>
  </ul>
</div>

## Introduction

HSP 2027 will bring together researchers working on human sentence processing, language comprehension and production, psycholinguistics, neurolinguistics, computational models of language processing, language acquisition, bilingualism, signed languages, and related areas of language and cognition.

The special theme for HSP 2027 is **Cognitive mechanisms of syntactic change throughout the lifespan**. We welcome submissions related to this theme as well as submissions on all aspects of human sentence processing.

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

Please contact us with any questions regarding the conference. Let us know what we can do to make the conference accessible to you.

**Email:** xxx
