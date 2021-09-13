<template>
  <main>
    <section class="self-center flex flex-col flex-1 items-center justify-center">
      <h1 class="title text-center">Mohibul Hassan Chowdhury</h1>
      <h5 class="subtitle text-center">Working as a Software Engineer</h2>
    </section>
    <section>
    <div>
    <IconLinkedin class="icon text-primary-400"/>
    </div>
    </section>

    <section class="mt-8">
      <h3 class="text-primary-600 dark:text-primary-400 max-w-5xl mx-auto">Latest blog post</h3>
      <posts post-type="blog" :amount="1" />
    </section>
  </main>
</template>
<script>
import IconLinkedin from '~/components/icons/linkedin.svg?inline'
export default {
  head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },

  components: {
    IconLinkedin
  }
}; 
</script>