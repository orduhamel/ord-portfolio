<template>
  <div class="inner-bloc">
    <figure class="visu-container">
      <img :src="project.url"/>
    </figure>
    <div class="text-container">
      <h3>{{ project.subTitle }}</h3>
      <h2>{{ project.title }}</h2>
      <p>{{ project.introduction }}</p>
      <p>{{ project.content }}</p>
    </div>
  </div>
</template>


<script>
  export default {
    data() {
      return {
        id: this.$route.params.id,
        projects: [
          {
            id: 'photographr',
            title: 'Photographr',
            subTitle: 'Ruby on Rails, JavaScript',
            introduction: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellendus velit unde facere, quibusdam odio provident illum maxime, voluptas, aliquam architecto ipsum corporis? Debitis officia, saepe laudantium eos architecto ipsa aperiam.',
            url: 'https://source.unsplash.com/random',
            content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Veritatis omnis, maxime repudiandae dicta aliquam error repellat minus deleniti ipsam ut sit dolorum non adipisci nobis voluptatem quia, sint est at!'
          },
          {
            id: 'bunnynb',
            title: 'Bunnynb',
            subTitle: 'Ruby on Rails, JavaScript',
            introduction: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellendus velit unde facere, quibusdam odio provident illum maxime, voluptas, aliquam architecto ipsum corporis? Debitis officia, saepe laudantium eos architecto ipsa aperiam.',
            url: 'https://source.unsplash.com/random',
            content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Veritatis omnis, maxime repudiandae dicta aliquam error repellat minus deleniti ipsam ut sit dolorum non adipisci nobis voluptatem quia, sint est at!'
          }
        ]
      }
    },
    computed: {
      project() {
        return this.projects.find(project => project.id == this.id)
      }
    }
  }
</script>

<style scoped>

</style>
