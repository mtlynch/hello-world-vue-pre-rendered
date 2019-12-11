<template>
  <div>
    <h1>Hello, world!</h1>
    <p>I'm an example of a pre-rendered Vue webpage.</p>
    <button v-on:click="count++">I have been clicked {{ count }} times</button>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      count: 0
    };
  }
};
</script>
