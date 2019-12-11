<template>
  <div>
    <h1>Hello, world!</h1>
    <p>I'm an example of a pre-rendered Vue webpage.</p>
    <p>
      To learn more, visit my
      <a href="https://github.com/mtlynch/hello-world-vue-static">Github repo</a
      >. or check the <nuxt-link to="/about">about page</nuxt-link>
    </p>
  </div>
</template>

<script>
export default {
  head: {
    // Sets the page's <title> tag.
    title: "Hello, World!"
  }
};
</script>
