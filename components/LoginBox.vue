<template>
  <div class="login-box">
    <a class="title">sign in</a>
  </div>
</template>

<script>
export default {
  name: 'LoginBox',
}
</script>

<style scoped>
.login-box {
  width: 300px;
  height: 330px;
  border: solid #857caf 1px;
  border-radius: 6px;
  background: #0e0f19;
  position: absolute;
  top: 50%;
  left: 50%;
  margin: -165px 0 0 -150px;
}
.title {
  text-align: center;
  display: block;
  top: 5px;
  margin-top: 5px;
}
</style>
