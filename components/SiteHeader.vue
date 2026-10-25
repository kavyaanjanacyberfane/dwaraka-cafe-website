<script setup lang="ts">
const menuOpen = ref(false);
const route = useRoute();
watch(() => route.fullPath, () => { menuOpen.value = false; });
const links = [{label:"Home",to:"/"},{label:"About",to:"/about"},{label:"Contact",to:"/contact"}];
</script>
<template>
<header class="site-header">
  <div class="container header-inner">
    <NuxtLink to="/" class="brand" aria-label="Dwaraka Cafe home"><img src="/images/dwaraka-cafe-logo.png" alt="Dwaraka Cafe Pure Veg logo" class="brand-logo" /></NuxtLink>
    <nav class="desktop-nav" aria-label="Main navigation">
      <NuxtLink v-for="link in links" :key="link.to" :to="link.to" :class="['nav-link',{active:route.path===link.to}]">{{link.label}}</NuxtLink>
      <NuxtLink to="/contact#visit" class="button button-small">Find Us ↗</NuxtLink>
    </nav>
    <button class="mobile-menu-button" type="button" :aria-expanded="menuOpen" aria-label="Toggle navigation" @click="menuOpen=!menuOpen"><span></span><span></span><span></span></button>
  </div>
  <Transition name="menu"><nav v-if="menuOpen" class="mobile-nav" aria-label="Mobile navigation">
    <NuxtLink v-for="link in links" :key="link.to" :to="link.to" class="mobile-nav-link">{{link.label}}</NuxtLink>
    <NuxtLink to="/contact#visit" class="button">Find Us ↗</NuxtLink>
  </nav></Transition>
</header>
</template>
