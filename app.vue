<template>

  <!-- WebGL Background -->
  <client-only>
    <LazyHero/>
  </client-only>

  <NuxtLayout>
    <NuxtPage/>
  </NuxtLayout>

  <!-- Dynamic Cursor Element -->
  <client-only>
    <LazyCursor/>
  </client-only>


</template>

<script setup>
import {useHead} from "nuxt/app";

useHead({
  title: 'Gideon Ramot | Front End Developer',
  viewport: 'width=device-width, initial-scale=1, maximum-scale=1',
  lang: 'en-US',
  charset: 'utf-8',
  htmlAttrs: {
    lang: 'en-US',
  },
  meta: [
    {
      hid: 'description',
      name: 'description',
      content: 'Hey I’m Gideon, and I\'m based in Semarang, Indonesia. My work revolves around creating unique interactive experiences with browser-based technology. I specialize in programming with React, Vue and Next although I come from an extensive UI/UX engineer background. I love writing code but I\'m also experienced in UI design, with a keen eye for detail and an understanding of interaction design and best practices. I often lead projects from ideation and architecture through implementation.'
    },
    {
      hid: 'theme-color',
      name: 'theme-color',
      content: '#12A9B2'
    },
    {
      hid: 'robots',
      name: 'robots',
      content: 'index, follow'
    },
    {
      hid: 'googlebot',
      name: 'googlebot',
      content: 'index, follow'
    },
    {
      hid: 'og:url',
      name: 'og:url',
      content: 'https://marchantweb.com'
    },
    {
      hid: 'og:title',
      name: 'og:title',
      content: 'Gideon Ramot | Front End Developer'
    },
    {
      hid: 'og:type',
      name: 'og:type',
      content: 'website'
    },
    {
      hid: 'og:image',
      name: 'og:image',
      content: 'https://marchantweb.com/cover.jpg'
    },
    {
      hid: 'og:image:alt',
      name: 'og:image:alt',
      content: 'Gideon Ramot | Front End Developer'
    },
    {
      hid: 'og:description',
      name: 'og:description',
      content: 'Hey I’m Gideon, and I\'m based in Semarang, Indonesia. My work revolves around creating unique interactive experiences with browser-based technology. I specialize in programming with React, Vue and Next although I come from an extensive UI/UX engineer background. I love writing code but I\'m also experienced in UI design, with a keen eye for detail and an understanding of interaction design and best practices. I often lead projects from ideation and architecture through implementation.'
    },
    {
      hid: 'og:site_name',
      name: 'og:site_name',
      content: 'Gideon Ramot | Front End Developer'
    },
    {
      hid: 'og:locale',
      name: 'og:locale',
      content: 'en_US'
    },
    {
      hid: 'twitter:card',
      name: 'twitter:card',
      content: 'summary_large_image'
    },
    {
      hid: 'twitter:site',
      name: 'twitter:site',
      content: '@marchantweb'
    },
    {
      hid: 'twitter:creator',
      name: 'twitter:creator',
      content: '@marchantweb'
    },
    {
      hid: 'twitter:url',
      name: 'twitter:url',
      content: 'https://marchantweb.com'
    },
    {
      hid: 'twitter:title',
      name: 'twitter:title',
      content: 'Gideon Ramot | Front End Developer'
    },
    {
      hid: 'twitter:description',
      name: 'twitter:description',
      content: 'Hey I’m Gideon, front end developer based in Semarang, Indonesia.'
    },
    {
      hid: 'twitter:image',
      name: 'twitter:image',
      content: 'https://marchantweb.com/cover.jpg'
    },
    {
      hid: 'twitter:image:alt',
      name: 'twitter:image:alt',
      content: 'Gideon Ramot | Front End Developer'
    }
  ],
  link: [
    {rel: 'icon', type: 'image/svg', href: '/icon-dark.svg'},
    {rel: 'preconnect', href: 'https://api.marchantweb.com'},
    {
      rel: 'stylesheet',
      href: 'https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,400;0,700;1,400;1,700&display=swap'
    },
    {rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap'},
  ],
  // script: [
  //   {
  //     src="https://kit.fontawesome.com/9f47c46af7.js", async: true, crossorigin: 'anonymous'
  //   }
  // ],
});
</script>
