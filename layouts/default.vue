<template>
  <div class="container min-w-full">
    <Navbar />
    <Nuxt />
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  background-size: cover;
  background-image: url('/background.jpg');
  background-repeat: no-repeat;
  background-position: 50% 70%;
  min-height: 100vh;
}

@media (max-width: 768px) {
  .container {
    background-position: 50% 50%;
    min-height: 100vh;
  }
}
</style>
