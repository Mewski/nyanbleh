<template>
  <div>
    <Navbar />
    <div class="content"></div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
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
.content {
  position: absolute;
  margin-top: 40px;
  animation: fadeInAnimation 1s ease 1 forwards;
}
</style>
