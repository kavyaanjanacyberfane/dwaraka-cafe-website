<script setup>
const siteUrl = "https://dwarakacafe.com",
  title = "Contact Dwaraka Cafe | Location & Phone",
  description =
    "Contact or find Dwaraka Cafe, a pure vegetarian restaurant in Patancheru Industrial Area, Hyderabad, Telangana 502319. Call 086394 08555.";
useSeoMeta({
  title,
  description,
  keywords:
    "Dwaraka Cafe contact, Dwaraka Cafe address, pure veg Patancheru phone",
  ogTitle: title,
  ogDescription: description,
  ogUrl: `${siteUrl}/contact`,
  ogImage: `${siteUrl}/images/dwaraka-cafe-logo.png`,
});
useHead({ link: [{ rel: "canonical", href: `${siteUrl}/contact` }] });
useSchemaOrg([
  defineWebPage({
    "@type": "ContactPage",
    "@id": `${siteUrl}/contact#webpage`,
    name: "Contact Dwaraka Cafe",
    description,
    url: `${siteUrl}/contact`,
  }),
  defineBreadcrumb({
    itemListElement: [
      { name: "Home", item: siteUrl },
      { name: "Contact", item: `${siteUrl}/contact` },
    ],
  }),
]);
</script>
<template>
  <div>
    <section class="inner-hero">
      <div class="container">
        <span class="kicker">SAY HELLO</span>
        <h1>We’d love to<br /><em>hear from you.</em></h1>
        <p>Planning a visit? Find our location or give us a call.</p>
      </div>
      <!-- <span class="hero-symbol">✳</span> -->
    </section>
    <section id="visit" class="section contact-section">
      <div class="container contact-grid">
        <div>
          <span class="kicker">GET IN TOUCH</span>
          <h2>Let’s make it<br /><em>a good visit.</em></h2>
          <p>We look forward to welcoming you to Dwaraka Cafe.</p>
          <div class="contact-item">
            <span class="contact-icon">⌖</span>
            <div>
              <small>OUR LOCATION</small>
              <p class="location-inline">
                <a
                  href="https://diningdistrict.in/"
                  target="_blank"
                  rel="noopener noreferrer"
                  class="dining-district-link"
                >
                  Dining District
                </a>
                <span>Patancheru Industrial Area, Hyderabad</span>
              </p>
              <a
                class="underlined"
                href="https://share.google/0XrmDYe0BPVJ77VJI"
                target="_blank"
                rel="noopener noreferrer"
                >Open directions ↗</a
              >
            </div>
          </div>
          <div class="contact-item">
            <span class="contact-icon">☎</span>
            <div>
              <small>CALL US</small><strong>086394 08555</strong>
              <p>Call us for enquiries before your visit.</p>
              <a class="underlined" href="tel:+918639408555"
                >Call Dwaraka Cafe ↗</a
              >
            </div>
          </div>
          <div class="contact-item">
            <span class="contact-icon">●</span>
            <div>
              <small>OUR FOOD</small><strong>Pure vegetarian</strong>
              <p>Vegetarian dishes in a welcoming setting.</p>
            </div>
          </div>
        </div>
        <div class="map-card">
          <div class="map-title">
            <span>⌖</span>
            <div>
              <small>COME FIND US</small>
              <h3>Dwaraka Cafe</h3>
              <p>
                <a
                  href="https://diningdistrict.in/"
                  target="_blank"
                  rel="noopener noreferrer"
                  class="dining-district-link"
                >
                  Dining District
                </a>
                <span>Patancheru Industrial Area, Hyderabad</span>
              </p>
            </div>
          </div>
          <div class="map-art">
            <div class="map-road road-a"></div>
            <div class="map-road road-b"></div>
            <div class="map-road road-c"></div>
            <div class="map-pin">✦</div>
            <span class="map-label">DWARAKA CAFE</span>
          </div>
          <a
            class="button map-button"
            href="https://share.google/0XrmDYe0BPVJ77VJI"
            target="_blank"
            rel="noopener noreferrer"
            >Open in Google Maps ↗</a
          >
          <p class="map-note">
            Directions open in Google Maps. Please confirm current opening hours
            directly with the restaurant.
          </p>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
/* Keep the About page layout centered */
/* About section layout */
.location-inline {
  display: flex;
  align-items: baseline;
  flex-wrap: wrap;
  gap: 8px;
}
.location-inline span {
  display: inline-block;
  font-size: 14px;
  font-weight: 700;
  color: var(--green) !important;
}

.dining-district-link {
  color: #b78116 !important;
  font-weight: 700;
  text-decoration: none;
  white-space: nowrap;
}

.dining-district-link:hover {
  color: #ffb51b !important;
  text-decoration: underline;
}
.about-grid {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  box-sizing: border-box;
  align-items: center;
}

/* Image container */
.about-photo-container {
  position: relative;
  width: 100%;
  height: 420px;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow: hidden;
  background: var(--green);
  text-align: center;
}

/* Image fills the container */
.about-photo-container .about-photo {
  display: block;
  width: 100%;
  max-width: none;
  height: 100%;
  max-height: none;
  margin: 0;
  object-fit: cover;
  object-position: center;
}

/* Mobile layout */
@media (max-width: 760px) {
  .about-grid {
    grid-template-columns: minmax(0, 1fr);
    gap: 30px;
    padding: 0 16px;
  }

  .about-photo-container {
    width: 100%;
    height: 340px;
  }
}

@media (max-width: 480px) {
  .about-grid {
    padding: 0 12px;
  }

  .about-photo-container {
    height: 280px;
  }
}
/* Make the restaurant image fill the entire container */
.about-photo-container .about-photo {
  display: block;
  width: 100%;
  max-width: none;
  height: 100%;
  max-height: none;
  margin: 0;
  object-fit: cover;
  object-position: center;
}

/* Caption overlay */
.about-photo-container .about-photo-caption {
  position: absolute;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 2;
  display: block;
  margin: 0;
  padding: 25px 12px 20px;
  color: #ffb51b;
  background: linear-gradient(
    to top,
    rgba(3, 59, 39, 0.95),
    rgba(3, 59, 39, 0)
  );
  font-size: 11px;
  font-weight: 800;
  letter-spacing: 0.16em;
  text-align: center;
}

/* Center the About section text */
.about-grid > div:last-child {
  text-align: center;
}

.about-grid > div:last-child .kicker {
  display: inline-block;
}

.about-grid > div:last-child h2 {
  text-align: center;
}

.about-grid > div:last-child p {
  max-width: 620px;
  margin: 0 auto 15px;
  text-align: center;
}

/* Center the vegetarian feature row */
.about-grid .fact {
  justify-content: center;
  text-align: left;
}

/* Center the page's top hero content */
.inner-hero > .container {
  text-align: center;
}

.inner-hero h1,
.inner-hero p {
  margin-right: auto;
  margin-left: auto;
}

.inner-hero p {
  max-width: 620px;
}

/* Tablet and mobile */
@media (max-width: 760px) {
  .about-grid {
    grid-template-columns: minmax(0, 1fr);
    gap: 30px;
  }

  .about-photo-container {
    height: 340px;
  }
}

@media (max-width: 480px) {
  .about-photo-container {
    height: 280px;
  }

  .about-grid > div:last-child h2 {
    font-size: clamp(30px, 8vw, 38px);
  }
}
</style>
