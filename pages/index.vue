<template>
  <div>
    <main>
      <section class="hero wrapper">
        <div class="titles">
          <h1>Fullstack developer</h1>
          <h2>I design and code beautifully simple things, and I love what I do.</h2>
        </div>
      </section>
      <div v-for="project in manifest" class="wrapper">
        <project-glimpse :title="project.title" :sub-title="project.subTitle" :description="project.description" :url="project.url" :link="project.link"></project-glimpse>
      </div>
    </main>
  </div>
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import ProjectGlimpse from '../components/index/ProjectGlimpse.vue'

  export default {
    components: {
      Logo,
      ProjectGlimpse
    },
    data() {
      return {
        manifest: [
          {
            title: 'Photographr',
            subTitle: 'Ruby on Rails, JavaScript',
            description: 'Hello World',
            url: 'https://source.unsplash.com/random',
            link: 'https://source.unsplash.com/random'
          },
          {
            title: 'Bunnynb',
            subTitle: 'Ruby on Rails, JavaScript',
            description: 'Hello World',
            url: 'https://source.unsplash.com/random',
            link: 'https://source.unsplash.com/random'
          }
        ]
      }
    }
  }
</script>

<style>
  .hero {
    min-height: 100vh;
    text-align: center;
    margin: 0 auto;
  }

</style>
