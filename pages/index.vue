<template>
  <div class="container">
    <header class="hero">
      <div class="hero-bg-wraper">
        <img src="../assets/images/hero-bg-image.jpg" alt="" class="header-bg-image">
      </div>
      <div class="titles">
        <h1>Ophelie Raymond-Duhamel</h1>
        <h2>Hi I’m a freelance coding designer with a natural attraction for interfaces, user intercations, marketing and branding.</h2>
        <nav class="header-nav">
          <ul class="list-horizontal">
            <li>
              <a href="#">Contact me</a>
            </li>
            <li>
              <a href="#skills">Discover my work and skills</a>
            </li>
          </ul>
        </nav>
      </div>
    </header>
    <main>
      <!-- Skills and tools -->
      <section class="skills">
        <div id="skills">

        </div>
      </section>
      <!-- About me and philosophy -->
      <section></section>
    </main>
    <div v-for="project in manifest" class="wrapper">
      <project-glimpse :title="project.title" :sub-title="project.subTitle" :description="project.description" :url="project.url" :link="project.link"></project-glimpse>
    </div>
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
    width: 100vh;
    text-align: center;
    margin: 0 auto;
    position: relative;
  }

  .hero-bg-wraper {
    positon: fixed;
    top: 0;
    left: 0;
    height: inherit;
    width: 100%;
  }

  .header-bg-image {
    position: relative;
    max-width: none;
    width: auto;
    height: 100%;
  }


</style>
