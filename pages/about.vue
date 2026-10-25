<script setup>
const siteUrl = "https://dwarakacafe.com",
  title = "About Dwaraka Cafe | Pure Vegetarian Restaurant",
  description =
    "Get to know Dwaraka Cafe, a pure vegetarian dining destination in Patancheru Industrial Area, Hyderabad.";
useSeoMeta({
  title,
  description,
  keywords:
    "about Dwaraka Cafe, pure vegetarian restaurant Hyderabad, Patancheru cafe",
  ogTitle: title,
  ogDescription: description,
  ogUrl: `${siteUrl}/about`,
  ogImage: `${siteUrl}/images/dwaraka-cafe-logo.png`,
});
useHead({ link: [{ rel: "canonical", href: `${siteUrl}/about` }] });
useSchemaOrg([
  defineWebPage({
    "@type": "AboutPage",
    "@id": `${siteUrl}/about#webpage`,
    name: "About Dwaraka Cafe",
    description,
    url: `${siteUrl}/about`,
  }),
  defineBreadcrumb({
    itemListElement: [
      { name: "Home", item: siteUrl },
      { name: "About", item: `${siteUrl}/about` },
    ],
  }),
]);
</script>
<template>
  <div>
    <section class="inner-hero">
      <div class="container">
        <span class="kicker">OUR STORY</span>
        <h1>A place for good food<br /><em>and good company.</em></h1>
        <p>
          At Dwaraka Cafe, we believe the best meals are the ones you enjoy
          together.
        </p>
      </div>
      <span class="hero-symbol">✳</span>
    </section>
    <section class="section">
      <div class="container about-grid">
        <div class="about-emblem">
          <img
            src="/images/dwaraka-cafe-logo.png"
            alt="Dwaraka Cafe logo"
          /><span>PURE VEG · WARM HEARTS</span>
        </div>
        <div>
          <span class="kicker">A WARM WELCOME</span>
          <h2>Vegetarian dining,<br /><em>with a little extra heart.</em></h2>
          <p>
            Dwaraka Cafe is a pure vegetarian restaurant in Patancheru
            Industrial Area, Hyderabad. We’re here to offer a welcoming place
            where friends, families, colleagues, and food lovers can come
            together over a meal.
          </p>
          <p>
            Whether you’re stopping by during a busy day or meeting the people
            who matter, we want your visit to feel comfortable, friendly, and
            worth repeating.
          </p>
          <div class="fact">
            <span>●</span>
            <div>
              <strong>Pure vegetarian</strong
              ><small>A vegetarian dining experience</small>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section values">
      <div class="container">
        <div class="center-heading">
          <span class="kicker">WHAT MATTERS TO US</span>
          <h2>Our kind of <em>hospitality.</em></h2>
        </div>
        <div class="cards">
          <article class="value-card">
            <span class="value-icon">✦</span>
            <h3>Welcoming everyone</h3>
            <p>
              A friendly place to gather, celebrate, and enjoy vegetarian food
              together.
            </p>
          </article>
          <article class="value-card featured">
            <span class="value-icon">✺</span>
            <h3>Food brings us closer</h3>
            <p>
              We believe meals create space for conversation, connection, and
              little everyday joys.
            </p>
          </article>
          <article class="value-card">
            <span class="value-icon">❋</span>
            <h3>Local at heart</h3>
            <p>
              Proud to welcome guests in the Patancheru Industrial Area of
              Hyderabad.
            </p>
          </article>
        </div>
      </div>
    </section>
    <section class="cta">
      <div class="container cta-inner">
        <div>
          <span class="kicker">WE’D LOVE TO WELCOME YOU</span>
          <h2>Come as you are.<br /><em>Leave with a smile.</em></h2>
        </div>
        <NuxtLink to="/contact" class="button button-light"
          >Contact us ↗</NuxtLink
        >
      </div>
    </section>
  </div>
</template>
