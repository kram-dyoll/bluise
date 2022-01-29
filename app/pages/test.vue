<template>
  <div>
    <h1>Test</h1>
    <button @click="functionTest">Fun times ahead</button>
  </div>
</template>

<script>
export default {
  methods: {
    functionTest () {
      //https://practical-shockley-347c4f.netlify.app/.netlify/functions/sharpspring-send
      fetch('https://agitated-perlman-9f9465.netlify.app/.netlify/functions/sharpspring-send')
        .then(response => response.json())
        .then(data => {
          console.log(data);
        });
    }
  }
}
</script>

<style scoped>

</style>
