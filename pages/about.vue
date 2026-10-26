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
      <!-- <span class="hero-symbol">✳</span> -->
    </section>
    <section class="section">
      <div class="container about-grid">
        <div class="about-emblem about-photo-container">
          <img
            src="https://b.zmtcdn.com/data/pictures/5/21221755/88518d419af1d6f7cab4f9a26c71580d.jpg?crop=700%3A400%3B%2A%2C%2A&fit=around%7C700%3A400&output-format=webp"
            alt="Dwaraka Cafe restaurant interior"
            class="about-photo"
          />

          <span class="about-photo-caption"> PURE VEG · WARM HEARTS </span>
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
<style scoped>
/* Keep the About page layout centered */
/* About section layout */
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
