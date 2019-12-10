<template>
  <div>
    <h1>About this Build</h1>
    <p>
      This page was rendered at <b>{{ buildTime }}</b
      >.
    </p>
    <p>
      This page was loaded at <b>{{ loadTime }}</b
      >.
    </p>
    <p><nuxt-link to="/">Home</nuxt-link></p>
  </div>
</template>

<script>
export default {
  head: {
    title: "About this Build"
  },
  // Vue evaluates asyncData once at page build time.
  asyncData() {
    return {
      buildTime: new Date()
    };
  },
  // Vue evaluates data variables at page render time and again every time the
  // browser loads this page.
  data: function() {
    return {
      loadTime: new Date()
    };
  }
};
</script>
