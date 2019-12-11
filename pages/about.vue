<template>
  <div>
    <h1>About this Build</h1>
    <p>
      This page was pre-rendered at <b>{{ buildTime }}</b
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
  asyncData() {
    // Don't re-evaluate buildTime when the client loads this page in the
    // browser.
    if (!process.client) {
      return {
        buildTime: new Date().toUTCString()
      };
    }
  },
  // Vue evaluates data variables at page render time and again every time the
  // browser loads this page.
  data: function() {
    return {
      loadTime: new Date().toUTCString()
    };
  }
};
</script>
