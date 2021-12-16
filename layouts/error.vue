<template>
  <div>
    <Navbar />
    <div class="content">
      <h1 v-if="error.statusCode === 404">Page not found</h1>
      <NuxtLink to="/">Home page</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  props: ['error'],
  layout: 'error', // you can set a custom layout for the error page
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@400&display=swap');
* {
  transition: 0.15s;
  font-family: 'Quicksand', sans-serif;
}
body {
  background-color: #14151f;
  margin: 0;
  padding: 0;
}
@keyframes fadeInAnimation {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
.content {
  position: absolute;
  margin-top: 40px;
  animation: fadeInAnimation 1s ease 1 forwards;
}
h1 {
  color: #dcdcdc;
  text-decoration: none;
}
</style>
