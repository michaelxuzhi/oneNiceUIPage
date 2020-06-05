<template>
  <div class="left-bot">
    <div class="item-margin" v-for="(item, index) in botList" :key="index">
      <i class="icon-margin" :class="item.icon"></i>
      {{ item.title }}
    </div>
  </div>
</template>
<script>
export default {
  name: 'leftBandBot',
  props: {
    botList: {
      default() {
        return []
      },
    },
  },
}
</script>
<style scoped>
.left-bot {
  color: rgb(155, 148, 148);
  padding: 5% 0 0 5%;
  /* background-color: rgb(53, 17, 17); */
}
.item-margin {
  padding-bottom: 15px;
  border-right: 3px solid #84fce2;
}
.icon-margin {
  padding-right: 10px;
}
</style>
