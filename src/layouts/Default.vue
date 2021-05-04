<template>
  <div class="container">
    <section class="hero is-primary">
      <div class="hero-body">
        <div class="columns">
          <div class="column is-full">
            <div class="media">
              <div class="media-left">
                <figure class="image is-96x96">
                  <g-image alt="Headshot" src="~/assets/images/headshot.jpg" class="is-rounded" />
                </figure>
              </div>
              <div class="media-content">
                <p class="title is-3 mt-5">Josh Burks</p>
                <p class="subtitle is-5">Sr. Software Developer</p>
              </div>
            </div>
          </div>
        </div>
        <div class="columns">
          <div class="column is-full">
            <nav class="breadcrumb is-pulled-right">
              <ul>
                <li><g-link to="/">About Me</g-link></li>
                <li><g-link to="/work-with-me">Work With Me</g-link></li>
                <li><g-link to="/contact">Contact Me</g-link></li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </section>
    <slot/>

    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          <a class="mr-5" href="mailto:joshburks@hey.com" target="_blank"><i data-feather="at-sign"></i></a>
          <a class="ml-5 mr-5" href="tel:870-403-2256" target="_blank"><i data-feather="smartphone"></i></a>
          <a class="ml-5 mr-5" href="https://github.com/dotnofoolin" target="_blank"><i data-feather="github"></i></a>
          <a class="ml-5 mr-5" href="https://www.linkedin.com/in/joshrburks/" target="_blank"><i data-feather="linkedin"></i></a>
          <a class="ml-5" href="https://twitter.com/joshrburks" target="_blank"><i data-feather="twitter"></i></a>
        </p>
      </div>
    </footer>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
  mounted() {
    this.$feather.replace()
  }
}
</script>

<style>
</style>
