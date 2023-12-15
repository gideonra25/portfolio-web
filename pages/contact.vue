<template>
  <section class="page">

    <div class="container-xxxl">
      <div class="row mt-0 mt-lg-6 justify-content-end">
        <div class="col-12 col-md-8 col-lg-7 col-xl-5 col-xxl-4 mb-4">
          <NuxtLink class="back-link mouse-md mt-4 mt-lg-0" to="/"><i class="fa-solid fa-chevron-left fa-2x pe-3"></i>Back
          </NuxtLink>
          <CodeTag class="mt-5 mb-3">contact</CodeTag>
          <h1 class="mb-4">Let's Chat</h1>
          <p class="mb-4">Feel free to get in touch anytime. I'm open to discussing ideas, feasibility, scheduling, and more. Whether you have questions or just want to say hello, that's great too.</p>
          <h2 class="mb-7"><a href="mailto:gideonnoedigp2504@gmail.com" target="blank" class="mouse-md"
                                style="color: #12A9B2">gideonnoedigp2504@gmail.com</a></h2>
          <h3 class="mb-3">Collaboration Session</h3>
          <p class="mb-4">If you want to dive more into project specifics, you can contact me for a further meeting, and see if we're a good fit.</p>
          <ActionButton to="https://wa.me/6289648410773" target="_blank">
            <i class="fa-solid fa-phone fa-lg"></i>
            Contact Me
          </ActionButton>
        </div>
        <div class="col-1 d-none d-xl-block"></div>
      </div>
    </div>

  </section>
</template>

<script setup>

import {useScriptTag} from '@vueuse/core'

useHead({
  title: 'Let\'s Chat - Collaboration Session | Gideon Ramot',
  meta: [
    {
      name: 'description',
      content: 'Schedule a one-hour initial discovery session for your project, or reach out via email.'
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
  transform: translateX(10%) translateZ(0);
  transform-origin: right center;
}

#calendar-container {
  height: 700px;
  width: 100%;
}

.back-link {
  color: #212A36;
  position: fixed;
  top: 40px;
  left: 60px;

  @media screen and (max-width: 992px) {
    position: relative;
    top: 0;
    left: 0;
  }
}

.container-xxxl {
  min-height: calc(100vh - 120px);
  display: flex;
  flex-direction: column;
  justify-content: center;

  @media screen and (max-width: 768px) {
    justify-content: flex-start;
    min-height: unset;
  }
}

</style>
