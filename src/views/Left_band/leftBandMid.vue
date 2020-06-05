<template>
  <div class="left-mid">
    <div class="item-margin" v-for="(item, index) in midList" :key="index">
      <i class="icon-margin" :class="item.icon"></i>{{ item.title }}
    </div>
  </div>
</template>
<script>
export default {
  name: 'leftBandMid',
  props: {
    midList: {
      default() {
        return []
      },
    },
  },
}
</script>
<style scoped>
.left-mid {
  color: rgb(255, 255, 255);
  padding: 5% 0 15% 5%;
  /* background-color: rgb(102, 66, 66); */
}
.item-margin {
  border-right: 3px solid #84fce2;
  padding-bottom: 15px;
}
.icon-margin {
  padding-right: 10px;
}
</style>
