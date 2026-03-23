<template>
  <Navbar />
  <Hero />
  <About />
  <Skills />
  <Services />
  <Projects />
  <Contact />
  <Footer />
</template>

<script setup>
import { watch } from 'vue';
import { useI18n } from 'vue-i18n';
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import About from './components/About.vue';
import Skills from './components/Skills.vue';
import Services from './components/Services.vue';
// import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';

const { locale, t } = useI18n();

watch(locale, (newLocale) => {
  document.documentElement.lang = newLocale;
  document.title = t('seo.title');
  
  const tagsToUpdate = {
    'meta[name="description"]': 'content',
    'meta[property="og:title"]': 'content',
    'meta[property="og:description"]': 'content',
    'meta[property="twitter:title"]': 'content',
    'meta[property="twitter:description"]': 'content'
  };

  for (const [selector, attr] of Object.entries(tagsToUpdate)) {
    const el = document.querySelector(selector);
    if (el) {
      if (selector.includes('title')) {
        el.setAttribute(attr, t('seo.title'));
      } else {
        el.setAttribute(attr, t('seo.description'));
      }
    }
  }
}, { immediate: true });
</script>

<style>
/* Base styles handled by linked CSS in index.html */
</style>
