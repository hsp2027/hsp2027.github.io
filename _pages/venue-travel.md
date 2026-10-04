---
layout: page
title: Venue & Travel
permalink: /venue-travel/
nav: true
nav_order: 3
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
    text-align: center;
  }

  .travel-page {
    font-size: 1rem;
    line-height: 1.65;
  }

  .travel-card {
    background: var(--global-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    box-shadow: 0 4px 14px rgba(0, 0, 0, 0.06);
    margin: 1.5rem 0;
    padding: 1.25rem;
  }

  .travel-card h2 {
    align-items: center;
    display: flex;
    font-size: 1.35rem;
    font-weight: 700;
    gap: 0.65rem;
    margin-top: 0;
    margin-bottom: 0.85rem;
  }

  .travel-card h2 i {
    color: var(--global-theme-color);
    font-size: 1.2rem;
    line-height: 1;
    text-align: center;
    width: 1.35rem;
  }

  .travel-card h3 {
    font-size: 1.05rem;
    font-weight: 700;
    margin-top: 1.2rem;
    margin-bottom: 0.35rem;
  }

  .travel-card p:last-child,
  .travel-card ul:last-child {
    margin-bottom: 0;
  }

  .travel-map iframe {
    border: 0;
    border-radius: 8px;
    min-height: 360px;
    width: 100%;
  }

  .travel-grid {
    display: grid;
    gap: 1rem;
    margin: 1rem 0;
  }

  .travel-airport {
    border-left: 3px solid var(--global-theme-color);
    padding-left: 0.85rem;
  }

  .travel-option {
    border-left: 3px solid var(--global-theme-color);
    padding-left: 0.85rem;
  }

  .travel-venue-grid {
    display: grid;
    gap: 1rem;
    grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
    margin-top: 0.25rem;
  }

  .travel-venue-item {
    background: color-mix(in srgb, var(--global-theme-color) 6%, transparent);
    border-left: 3px solid var(--global-theme-color);
    border-radius: 6px;
    padding: 0.85rem 0.95rem;
  }

  .travel-venue-item strong {
    display: block;
    margin-bottom: 0.25rem;
  }

  .travel-airport-title {
    display: block;
    font-size: 1rem;
    font-weight: 700;
    margin-top: 0;
    margin-bottom: 0.35rem;
  }

  .travel-option-title {
    display: block;
    font-size: 1rem;
    font-weight: 700;
    margin-top: 0;
    margin-bottom: 0.35rem;
  }

  .travel-table-wrap {
    overflow-x: auto;
  }

  .travel-table {
    margin: 0.85rem 0 0;
    min-width: 720px;
    width: 100%;
  }

  .travel-table th,
  .travel-table td {
    border-bottom: 1px solid var(--global-divider-color);
    padding: 0.55rem 0.65rem;
    vertical-align: top;
  }

  .travel-table th {
    font-weight: 700;
  }

  .travel-note {
    color: var(--global-text-color-light);
    font-size: 0.95rem;
  }

  .travel-jump {
    align-items: center;
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem 0.7rem;
    justify-content: center;
    margin: -0.25rem 0 1.5rem;
  }

  .travel-jump a {
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.92rem;
    padding: 0.2rem 0.65rem;
  }

  .travel-jump-label {
    color: var(--global-text-color-light);
    font-size: 0.92rem;
    font-weight: 600;
  }

  .travel-address {
    color: var(--global-text-color-light);
    display: block;
    font-size: 0.92rem;
    margin-top: 0.15rem;
  }

  .travel-map-title {
    font-size: 1.05rem;
    font-weight: 700;
    margin-top: 1.5rem;
    margin-bottom: 0.65rem;
  }
</style>

<h1 class="hsp-page-title">Venue & Travel Guide</h1>

<div class="travel-page" markdown="1">

<nav class="travel-jump" aria-label="Venue and travel page sections">
  <span class="travel-jump-label">Jump to:</span>
  <a href="#conference-venue">Conference Venue</a>
  <a href="#getting-to-campus">Getting to Campus</a>
  <a href="#accommodation">Accommodation</a>
  <a href="#campus-local-highlights">Campus and Local Highlights</a>
</nav>

<section id="conference-venue" class="travel-card">
  <h2><i class="fa-solid fa-location-dot" aria-hidden="true"></i>Conference Venue</h2>
  <div class="travel-venue-grid">
    <div class="travel-venue-item">
      <strong>Keynote presentations</strong>
      TBD
    </div>
    <div class="travel-venue-item">
      <strong>Poster sessions</strong>
      Stewart Center (STEW), Room 214
      <span class="travel-address">28 Memorial Mall Dr STEW G054, West Lafayette, IN 47907</span>
    </div>
    <div class="travel-venue-item">
      <strong>Reception</strong>
      South Ballroom, Purdue Memorial Union
      <span class="travel-address">101 Grant St, West Lafayette, IN 47906</span>
    </div>
  </div>

  <div class="travel-map">
    <div class="travel-map-title">Map of Conference Venues and Important Locations</div>
    <p class="travel-note">
      <a href="https://umap.openstreetmap.fr/en/map/hsp-2027_1436646?scaleControl=false&miniMapControl=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true" target="_blank" rel="noopener">Open the full-screen map</a> to view the primary conference venues, nearby parking areas, and hotel locations in greater detail.
    </p>
    <iframe
      title="Map of HSP 2027 conference venues and important locations"
      allowfullscreen
      allow="geolocation"
      src="https://umap.openstreetmap.fr/en/map/hsp-2027_1436646?scaleControl=false&miniMapControl=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true"
    ></iframe>
  </div>
</section>

<section id="getting-to-campus" class="travel-card">
  <h2><i class="fa-solid fa-plane-arrival" aria-hidden="true"></i>Getting to Campus</h2>

  <h3>By Air</h3>
  <div class="travel-grid">
    <div class="travel-airport">
      <strong class="travel-airport-title">Purdue University Airport (LAF)</strong>
      <p>LAF is located on campus, about a five-minute drive from the main conference area.</p>
    </div>
    <div class="travel-airport">
      <strong class="travel-airport-title">Indianapolis International Airport (IND)</strong>
      <p>IND is about 1 hour and 15 minutes from Purdue's campus.</p>
    </div>
    <div class="travel-airport">
      <strong class="travel-airport-title">Chicago O'Hare International Airport (ORD)</strong>
      <p>ORD is about 2 hours and 15 minutes from Purdue's campus.</p>
    </div>
  </div>

  <p>Rental cars are available at both IND and ORD.</p>
  <p>Shuttle services connect the airports with West Lafayette. Please check schedules and book tickets in advance through <a href="https://www.reindeershuttle.com/" target="_blank" rel="noopener">Reindeer Shuttle</a> or <a href="https://www.lafayettelimo.com/services/indianapolis-airport-shuttle-service" target="_blank" rel="noopener">Lafayette Limo</a>.</p>

  <h3>By Car</h3>
  <p>Visitors have several parking options on and around campus:</p>
  <div class="travel-grid">
    <div class="travel-option">
      <strong class="travel-option-title">Parking garages</strong>
      <p>The Grant Street Parking Garage (120 North Grant Street) and Harrison Street Parking Garage (719 Clinic Drive) are available for campus visitors. Motorists may park in either garage for up to 24 hours at a time. Garage rates are $2.00 for 0-30 minutes, $5.00 for 30-60 minutes, $2.00 for each additional hour, and $20.00 for the full 24 hours.</p>
    </div>
    <div class="travel-option">
      <strong class="travel-option-title">Daily visitor parking pass</strong>
      <p>Visitors may purchase a daily visitor pass through the <a href="https://purdue.t2hosted.com/Account/Portal" target="_blank" rel="noopener">Purdue Parking Portal</a>, which allows parking in eligible A, B, or C lots. These passes are $8.00 per day.</p>
    </div>
    <div class="travel-option">
      <strong class="travel-option-title">Metered street parking</strong>
      <p>Metered street parking is available throughout campus.</p>
    </div>
  </div>
</section>

<section id="accommodation" class="travel-card">
  <h2><i class="fa-solid fa-hotel" aria-hidden="true"></i>Accommodation</h2>
  <p>At this time, we have no conference-rate agreements for lodging. The hotels below receive positive online ratings and represent a range of price points.</p>

  <div class="travel-table-wrap">
    <table class="travel-table">
      <thead>
        <tr>
          <th>Hotel / Booking Link</th>
          <th>Distance</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><a href="https://www.marriott.com/en-us/hotels/indwk-the-union-club-hotel-at-purdue-university-autograph-collection/overview/" target="_blank" rel="noopener">The Union Club Hotel at Purdue University, Autograph Collection</a></td>
          <td>Walkable</td>
        </tr>
        <tr>
          <td><a href="https://www.hilton.com/en/hotels/lafwehx-hampton-suites-west-lafayette/" target="_blank" rel="noopener">Hampton Inn &amp; Suites by Hilton West Lafayette</a></td>
          <td>Walkable</td>
        </tr>
        <tr>
          <td><a href="https://www.hilton.com/en/hotels/lafwlgi-hilton-garden-inn-west-lafayette-wabash-landing/" target="_blank" rel="noopener">Hilton Garden Inn West Lafayette Wabash Landing</a></td>
          <td>Walkable</td>
        </tr>
        <tr>
          <td><a href="https://www.druryhotels.com/locations/lafayette-in/drury-inn-and-suites-lafayette-in" target="_blank" rel="noopener">Drury Inn &amp; Suites Lafayette, IN</a></td>
          <td>Less than 5 miles from campus</td>
        </tr>
        <tr>
          <td><a href="https://www.ihg.com/holidayinn/hotels/us/en/lafayette/lafin/hoteldetail" target="_blank" rel="noopener">Holiday Inn Lafayette-City Centre</a></td>
          <td>Less than 5 miles from campus</td>
        </tr>
        <tr>
          <td><a href="https://www.marriott.com/en-us/hotels/lafcy-courtyard-lafayette/overview/" target="_blank" rel="noopener">Courtyard by Marriott Lafayette</a></td>
          <td>Less than 5 miles from campus</td>
        </tr>
        <tr>
          <td><a href="https://www.vrbo.com/en-ca/vacation-rentals/united-states/indiana/tippecanoe-county/west-lafayette/purdue-university" target="_blank" rel="noopener">Vrbo options near Purdue University</a></td>
          <td>Variable</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

<section id="campus-local-highlights" class="travel-card">
  <h2><i class="fa-solid fa-star" aria-hidden="true"></i>Campus and Local Highlights</h2>

  <h3>Purdue Campus</h3>
  <ul>
    <li><strong><a href="https://www.google.com/maps/search/?api=1&query=Stewart+Center%2C+128+Memorial+Mall%2C+West+Lafayette%2C+IN+47907" target="_blank" rel="noopener">Stewart Center</a>:</strong> Home to the Purdue Welcome Center and Purdue Team Store, a handy stop if you would like to learn more about the university or pick up Boilermaker gear.</li>
    <li><strong><a href="https://www.purdue.edu/operations/pmu/" target="_blank" rel="noopener">Purdue Memorial Union</a>:</strong> The closest and most convenient place to eat near the conference venue. The ground floor has many dining options, and the building also includes a hotel and <a href="https://events.purdue.edu/purdue_memorial_union" target="_blank" rel="noopener">activities</a> such as bowling at Union Rack and Roll.</li>
    <li><strong><a href="https://www.purdue.edu/operations/sustainable-ops/home/initiatives/farmers-market/" target="_blank" rel="noopener">The Purdue Farmers Market</a>:</strong> Held at Memorial Mall on Thursdays from 11 a.m. to 3 p.m. during the season. It hosts several vendors offering local fresh produce, herbs, plants and flowers, meats, and prepared food, including lunches and sweets. Please check the official site for the current schedule.</li>
    <li><strong><a href="https://www.cla.purdue.edu/academic/rueffschool/galleries/index.html" target="_blank" rel="noopener">Robert L. Ringel Gallery</a>:</strong> Located in Stewart Center, one floor below the HSP poster sessions, with regional and international art as well as work by Purdue visual arts scholars.</li>
    <li><strong><a href="https://www.cla.purdue.edu/academic/rueffschool/collections/degas/index.html" target="_blank" rel="noopener">Degas sculpture collection</a>:</strong> A permanent collection on the second floor of Purdue Memorial Union.</li>
    <li><strong><a href="https://www.arboretum.purdue.edu/come-learn/horticulture-park/" target="_blank" rel="noopener">Purdue Horticulture Park</a> and campus routes:</strong> Easy options for a morning jog or walk through campus architecture and local flora.</li>
  </ul>

  <h3>West Lafayette and Lafayette</h3>
  <ul>
    <li><strong><a href="https://www.homeofpurdue.com/downtown/" target="_blank" rel="noopener">Historic downtown Lafayette</a>:</strong> Local businesses, restaurants, and a bit of midwestern charm across the river from campus.</li>
    <li><strong><a href="https://www.artlafayette.org/" target="_blank" rel="noopener">Art Museum of Greater Lafayette</a> and <a href="https://thehaan.org/" target="_blank" rel="noopener">Haan Museum of Indiana Art</a>:</strong> Two local art museums to explore during downtime.</li>
    <li><strong><a href="https://lafayette-symphony-orchestra.my.salesforce-sites.com/ticket/#/instances/a0FUu000009J2ddMAC" target="_blank" rel="noopener">Lafayette Symphony Orchestra</a>:</strong> Pianist Tuffus Zimbabwe will perform with the orchestra on Thursday, May 20.</li>
    <li><strong><a href="https://visitwolfpark.org/" target="_blank" rel="noopener">Wolf Park</a>:</strong> A conservation center in Battle Ground, Indiana, about a 15-minute drive from campus, where visitors can learn about wolves, foxes, and bison.</li>
  </ul>
</section>

</div>
