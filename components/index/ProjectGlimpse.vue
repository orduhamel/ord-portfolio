<template>
  <div class="inner-bloc">
    <div class="visu-container">
      <img :src="url" width="235" height="300"/>
    </div>
    <div class="text-container">
      <h3>{{ subTitle }}</h3>
      <h2>{{ title }}</h2>
      <p>{{ description }}</p>
      <a :href="link">Click on me</a>
    </div>
  </div>
</template>


<script>
  export default {
    props: {
      title: {
        type: String,
        required: true,
        default: 'JavaScript'
      },
      subTitle: {
        type: String,
        required: true,
        default: 'My Project'
      },
      description: {
        type: String,
        required: true,
        default: 'Learning project'
      },
      url: {
        type: String
      },
      link: {
        type: String
      }
    }
  }
</script>

<style scoped>
  .inner-bloc {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    flex-wrap: wrap;
  }

</style>
