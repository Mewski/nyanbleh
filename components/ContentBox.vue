<template>
  <div class="box">
    <a class="title">Projects</a>
    <a class="content">Random Thing</a>
  </div>
</template>

<script>
export default {
  name: 'ContentBox',
}
</script>

<style scoped>
.box {
  border: solid 1px;
  border-radius: 8px;
  background-color: #0e0f19;
  border-color: #857caf;
  width: 250px;
  height: 300px;
  left: 65px;
  top: 65px;
  position: absolute;
  padding-right: 3px;
  padding-left: 3px;
}
.title {
  color: #dcdcdc;
  font-size: 16px;
  text-align: center;
  width: 100%;
  padding-top: 10px;
  position: absolute;
}
.content {
  color: #dcdcdc;
  font-size: 14px;
  text-align: center;
  width: 100%;
  position: absolute;
  display: inline-block;
}
</style>
