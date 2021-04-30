<template>
  <Layout>

    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
    <g-image alt="Example image" src="~/favicon.png" width="135" />

    <h1>Hello, world!</h1>

    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur excepturi labore tempore expedita, et iste tenetur suscipit explicabo! Dolores, aperiam non officia eos quod asperiores
    </p>

    <p class="home-links">
      <a href="https://gridsome.org/docs/" target="_blank" rel="noopener">Gridsome Docs</a>
      <a href="https://github.com/gridsome/gridsome" target="_blank" rel="noopener">GitHub</a>
    </p>

    <button class="button is-primary"><i data-feather="circle"></i>Click me</button>

    <div class="box"><p>Some cool content</p></div>
    <i data-feather="circle"></i>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  mounted() {
    // TODO: Figure out why HMR doesn't run this. Have to refresh the page in browser to pickup icon changes.
    this.$feather.replace()
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
