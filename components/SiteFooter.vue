<template>
  <footer class="site-footer">
    <div class="container footer-grid">
      <div>
        <img
          src="/images/dwaraka-cafe-logo.png"
          alt="Dwaraka Cafe Pure Veg"
          class="footer-logo"
        />
        <p>Good food, warm hospitality, and a pure vegetarian experience.</p>
      </div>

      <div class="footer-col">
        <h3>Explore</h3>
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/about">About us</NuxtLink>
        <NuxtLink to="/contact">Contact</NuxtLink>
      </div>

      <div class="footer-col">
        <h3>Visit Us</h3>

        <p>
          <a
            href="https://diningdistrict.in/"
            target="_blank"
            rel="noopener noreferrer"
            class="dining-district-link"
          >
            Dining District,
          </a>
          Patancheru Industrial Area,<br />
          Hyderabad, Telangana 502319
        </p>

        <a href="tel:+918639408555">086394 08555</a>

        <a
          href="https://share.google/0XrmDYe0BPVJ77VJI"
          target="_blank"
          rel="noopener noreferrer"
        >
          Google Maps ↗
        </a>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="container footer-bottom-inner">
        <span>
          © {{ new Date().getFullYear() }} Dwaraka Cafe. All rights reserved.
        </span>
        <span>● Pure Vegetarian</span>
      </div>
    </div>
  </footer>
</template>
