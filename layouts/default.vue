<template>
  <div class="container">
    <nuxt />
  </div>
</template>

<style>
@import url("https://use.typekit.net/qmb1rig.css");

html {
  --masqualero-font: masqualero, sans-serif;
  --roc-grotesk-font: roc-grotesk, sans-serif;
  font-family: var(--roc-grotesk-font);
  font-weight: 300;
  font-style: normal;
  font-size: 16px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

h1 {
  font-family: var(--masqualero-font);
  font-size: 70px;
  font-weight: 400;
  line-height: 1em;
}

h2 {
  font-family: var(--roc-grotesk-font);
  font-weight: 300;
  font-size: 20px;
}

main {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-wrap: wrap;
}

a {
  display: block;
}

.wrapper {
  width: 100%;
}



</style>
