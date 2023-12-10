<template>
  <section class="page">

    <div class="container-xxxl">
      <div class="row mt-0 mt-lg-6">
        <main class="d-flex flex-column" itemscope itemtype="https://schema.org/Person">
          <div class="col-12 col-md-8 col-lg-7 col-xl-6 col-xxl-5 mb-4">
            <NuxtLink class="back-link mouse-md mt-4 mt-lg-0 mb-5 mb-lg-0 d-block text-end text-md-start" to="/">Back<i
                class="fa-sharp fa-solid fa-arrow-up-right fa-2x ps-3"></i></NuxtLink>
            <CodeTag class="mt-5 mb-5 d-none d-lg-block">about</CodeTag>
            <div class="d-flex flex-row align-items-center mb-5">
              <img src="~assets/images/headshot.jpg" alt="Hey I'm Simon" class="headshot me-4 me-lg-5">
              <div>
                <h1 class="mb-1" itemprop="name">Gideon Ramot A P</h1>
                <StatusIndicator type="dark"/>
              </div>
            </div>
            <h2 class="my-4" itemprop="description">Front end developer with enthusiasm for designing and programming reative websites / applications.</h2>
            <div itemprop="knowsAbout">
              <p>
                Hey I’m Gideon, and I'm based in Semarang, Indonesia. My work revolves around creating
                unique interactive experiences with browser-based technology. I specialize in <a href="https://react.dev/" target="_blank" class="mouse-sm">React</a>/<a
                  href="https://vuejs.org/" target="_blank" class="mouse-sm">Vue</a>, and <a
                  href="https://nextjs.org/"
                  target="_blank"
                  class="mouse-sm">Next</a>,
                although I come from an extensive UI/UX engineer background.
              </p>
              <p>
                I love writing code but I'm also experienced in UI design, with a keen eye for detail and a deep
                understanding of best practices. I often lead projects from ideation and architecture throughimplementation.
              </p>
            </div>
            <h3 class="mt-5 mb-4">Journey’s Mate</h3>
            <p class="mb-4">
              My journey about Front End Specialist, towards what I dream of is not easy, I got Journey’s mate on that journey, such as:
            </p>
          </div>
          <div class="col-12 col-md-8 col-lg-7 col-xl-6 col-xxxl-6">
            <div class="client-logo__container">
              <img src="~/assets/images/clients/html.svg" alt="HTML logo" class="client-logo mouse-md">
              <img src="~/assets/images/clients/css.svg" alt="CSS logo" class="client-logo mouse-md">
              <img src="~/assets/images/clients/js.svg" alt="JS logo" class="client-logo mouse-md">
              <img src="~/assets/images/clients/ts.svg" alt="TS logo" class="client-logo mouse-md">
              <img src="~/assets/images/clients/figma.svg" alt="Figma logo" class="client-logo mouse-md">
              <img src="~/assets/images/clients/tailwind.svg" alt="Tailwind logo" class="client-logo mouse-md">
              <img src="~/assets/images/clients/react.svg" alt="React logo"
                   class="client-logo mouse-md">
              <img src="~/assets/images/clients/vue.svg" alt="Vue logo"
                   class="client-logo mouse-md">
              <img src="~/assets/images/clients/next.svg" alt="Next logo"
                   class="client-logo mouse-md">
              <img src="~/assets/images/clients/nuxt.svg" alt="Nuxt logo" class="client-logo mouse-md">
            </div>
          </div>
          <div class="col-12 col-md-8 col-lg-7 col-xl-6 col-xxl-5 mb-4 mb-lg-8">
            <h3 class="mt-5 mb-4">
              Get in Touch
            </h3>
            <p class="mb-5">
              Thanks for reading a little bit about me. I’m always happy to chat and provide any helpful advice that I
              can. You can contact me to see if we’re a good fit, or just email at <a
                href="mailto:gideonnoedigp2504@gmail.com" class="mouse-sm" itemprop="email">gideonnoedigp2504@gmail.com</a>.
            </p>
            <ActionButton to="/contact" data-aos="fade-up" class="d-none d-lg-block">
              <i class="fa-sharp fa-solid fa-comment"></i>
              Let's Chat
            </ActionButton>
          </div>
        </main>

      </div>
    </div>

  </section>
</template>

<script setup>

useHead({
  title: 'Hey, I\'m Gideon | Front End Developer',
  meta: [
    {
      name: 'description',
      content: 'Front end developer with enthusiasm for designing and programming reative websites / applications.'
    }
  ],
  bodyAttrs: {
    class: 'enable-scroll fixed-webgl'
  }
});

</script>

<style lang="scss" scoped>

.page-enter-active {
  transition: all 1.5s cubic-bezier(0.4, 0, 0, 1);
  transition-delay: 0.5s;
}

.page-leave-active {
  transition: all 1s;
}

.page-enter-from,
.page-leave-to {
  opacity: 0;
  transform: translateX(-10%) translateZ(0);
  transform-origin: left center;
}

.client-logo__container {
  display: grid;
  gap: 5px;
  grid-template-columns: repeat(5, 1fr);

  @media screen and (max-width: 1200px) {
    grid-template-columns: repeat(4, 1fr);
  }

  @media screen and (max-width: 992px) {
    grid-template-columns: repeat(3, 1fr);
  }

  &:hover {
    .client-logo:not(:hover) {
      opacity: 0.2;
    }
  }
}

.client-logo {
  width: 100%;
  opacity: 1;
  transition: opacity 0.3s ease;
}

.back-link {
  color: #212A36;
  position: fixed;
  top: 40px;
  right: 60px;

  @media screen and (max-width: 992px) {
    position: relative;
    top: 0;
    left: 0;
  }
}

.headshot {
  width: 100px;
  border-radius: 50%;

  @media screen and (max-width: 992px) {
    width: 70px;
  }
}

</style>
