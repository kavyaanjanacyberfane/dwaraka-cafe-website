<script setup>
const siteUrl = "https://dwarakacafe.com";
const title = "Dwaraka Cafe | Pure Veg Restaurant in Patancheru, Hyderabad";
const description =
  "Visit Dwaraka Cafe for a welcoming pure vegetarian dining experience in Patancheru Industrial Area, Hyderabad, Telangana.";
useSeoMeta({
  title,
  description,
  keywords:
    "Dwaraka Cafe, pure veg restaurant, vegetarian restaurant, Patancheru, Hyderabad",
  ogTitle: title,
  ogDescription: description,
  ogType: "website",
  ogUrl: siteUrl,
  ogImage: `${siteUrl}/images/dwaraka-cafe-logo.png`,
  twitterCard: "summary_large_image",
});
useHead({ link: [{ rel: "canonical", href: siteUrl }] });
useSchemaOrg([
  defineWebPage({
    "@type": "WebPage",
    "@id": `${siteUrl}/#webpage`,
    name: "Home",
    description,
    url: siteUrl,
  }),
  defineWebSite({
    "@type": "WebSite",
    "@id": `${siteUrl}/#website`,
    name: "Dwaraka Cafe",
    url: siteUrl,
    description,
  }),
defineLocalBusiness({
  "@type": "Restaurant",
  "@id": `${siteUrl}/#restaurant`,
  name: "Dwaraka Cafe",
  url: siteUrl,
  image: `${siteUrl}/images/dwaraka-cafe-logo.png`,
  logo: `${siteUrl}/images/dwaraka-cafe-logo.png`,
  telephone: "+91 86394 08555",
  servesCuisine: ["Vegetarian", "Indian"],
  address: {
    "@type": "PostalAddress",
    streetAddress: "Patancheru Industrial Area",
    addressLocality: "Hyderabad",
    addressRegion: "Telangana",
    postalCode: "502319",
    addressCountry: "IN",
  },
}),
  defineBreadcrumb({ itemListElement: [{ name: "Home", item: siteUrl }] }),
]);
</script>
<template>
  <div>
    <section class="hero">
      <div class="container hero-grid">
        <div class="hero-copy">
          <span class="eyebrow">✦ PURE VEGETARIAN · MADE WITH CARE</span>
          <h1>
            A little more <em>flavour.</em><br />A lot more <em>feeling.</em>
          </h1>
          <p>
            Welcome to Dwaraka Cafe — a place to slow down, share a meal, and
            enjoy the goodness of vegetarian food.
          </p>
          <div class="actions">
            <NuxtLink to="/contact#visit" class="button"
              >Plan Your Visit ↗</NuxtLink
            ><NuxtLink to="/about" class="text-link">Get to know us →</NuxtLink>
          </div>
          <div class="promise">
            <span>✦</span>
            <div>
              <strong>100% vegetarian</strong
              ><small>A welcoming place for every meal</small>
            </div>
          </div>
        </div>
        <div class="hero-art">
          <div class="hero-art-inner">
            <img
              src="/images/dwaraka-cafe-logo.png"
              alt="Dwaraka Cafe Pure Veg logo"
            />
            <div class="art-caption">
              ✦ &nbsp; PURE VEG · GOOD MOOD &nbsp; ✦
            </div>
          </div>
          <div class="floating-note">✳ Freshly welcoming</div>
        </div>
      </div>
    </section>
    <section class="section welcome">
      <div class="container two-col">
        <div>
          <span class="kicker">A TASTE OF DWARAKA</span>
          <h2>Vegetarian food.<br /><em>Made for togetherness.</em></h2>
        </div>
        <div>
          <p>
            Some meals are about more than what’s on the plate. They’re about
            conversations that run long, family moments, and the comfort of
            sharing something delicious.
          </p>
          <p>
            At Dwaraka Cafe, we welcome you to enjoy a relaxed pure vegetarian
            dining experience in Patancheru, Hyderabad.
          </p>
          <NuxtLink to="/about" class="underlined">Our story ↗</NuxtLink>
        </div>
      </div>
    </section>
    <section class="section values">
      <div class="container">
        <div class="center-heading">
          <span class="kicker">THE DWARAKA FEELING</span>
          <h2>Simple things, <em>done with heart.</em></h2>
          <p>
            A friendly space for good food and the people you love sharing it
            with.
          </p>
        </div>
        <div class="cards">
          <article class="value-card">
            <span class="value-icon">✺</span><small>01 / OUR PROMISE</small>
            <h3>Pure vegetarian</h3>
            <p>
              A vegetarian dining experience that makes everyone at the table
              feel welcome.
            </p>
          </article>
          <article class="value-card featured">
            <span class="value-icon">❋</span><small>02 / OUR APPROACH</small>
            <h3>Made for sharing</h3>
            <p>
              Bring your family, meet your friends, or simply take a break and
              enjoy the moment.
            </p>
          </article>
          <article class="value-card">
            <span class="value-icon">✦</span><small>03 / OUR PLACE</small>
            <h3>Warm hospitality</h3>
            <p>
              A relaxed place to gather, catch up, and make your everyday meal
              feel special.
            </p>
          </article>
        </div>
      </div>
    </section>
    <section class="cta">
      <div class="container cta-inner">
        <div>
          <span class="kicker">COME ON IN</span>
          <h2>Good food is better <em>together.</em></h2>
          <p>Find Dwaraka Cafe in Patancheru Industrial Area, Hyderabad.</p>
        </div>
        <NuxtLink to="/contact#visit" class="button button-light"
          >Get directions ↗</NuxtLink
        >
      </div>
    </section>
    <section class="section review">
      <div class="container review-grid">
        <div>
          <span class="kicker">YOUR WORDS MATTER</span>
          <h2>Enjoyed your visit?<br /><em>Tell us about it.</em></h2>
          <p>
            Your feedback helps us keep making every visit a better experience.
            Share your thoughts on Google.
          </p>
          <a
            class="button"
            href="https://share.google/0XrmDYe0BPVJ77VJI"
            target="_blank"
            rel="noopener noreferrer"
            >Find us on Google ↗</a
          >
        </div>
        <div class="poster-wrap">
          <img
            src="/images/google-review-poster.png"
            alt="Dwaraka Cafe Google review poster"
          />
        </div>
      </div>
    </section>
  </div>
</template>
