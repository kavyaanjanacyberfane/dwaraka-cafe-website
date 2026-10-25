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
      <span class="hero-symbol">✳</span>
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
              <small>OUR LOCATION</small
              ><strong>Patancheru Industrial Area</strong>
              <p>Hyderabad, Telangana 502319, India</p>
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
              <p>Patancheru Industrial Area, Hyderabad</p>
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
