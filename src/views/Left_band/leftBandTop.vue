<template>
  <div class="left-top">
    <img src="../../assets/img/1-5.jpg" alt="头像" />
  </div>
</template>
<script>
export default {
  name: 'leftBandTop',
}
</script>
<style scoped>
.left-top {
  padding-left: 20px;
  padding-bottom: 30px;
  height: 50px;
  position: relative;
  /* background-color: rgb(175, 156, 156); */
}
.left-top img {
  position: absolute;
  bottom: 30px;
  border-radius: 50%;
  height: 30px;
}
</style>
