<template>
  <div class="container">
    <section class="hero is-primary">
      <div class="hero-body">
        <div class="columns">
          <div class="column is-half">
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
          <div class="column is-half">
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
