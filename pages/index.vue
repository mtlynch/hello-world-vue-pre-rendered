<template>
  <div>
    <h1>Hello, world!</h1>
    <p>I'm an example of a pre-rendered Vue webpage.</p>
    <p>
      To learn more, visit my
      <a v-bind:href="repoUrl">Github repo</a>
      or check the <nuxt-link to="/about">about page</nuxt-link>.
    </p>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      repoUrl: "https://github.com/mtlynch/hello-world-vue-static"
    };
  }
};
</script>
