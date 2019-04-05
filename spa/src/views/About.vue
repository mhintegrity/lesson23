<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button v-on:click="goHome">Back Home</button>
  </div>
</template>

<script>
export default {
  name: 'about',
  methods: {
    goHome: function() {
      // named route using an object
      this.$router.push({ name: 'home' });
    }
  }
}
</script>