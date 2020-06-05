<template>
  <div class="leftBand">
    <left-band-top></left-band-top>
    <left-band-mid :midList="midList"></left-band-mid>
    <left-band-bot :botList="botList"></left-band-bot>
  </div>
</template>
<script>
import leftBandTop from './leftBandTop'
import leftBandMid from './leftBandMid'
import leftBandBot from './leftBandBot'
export default {
  name: 'leftBand',
  data() {
    return {
      midList: [
        {
          icon: '',
          title: 'Browser',
        },
        {
          icon: 'el-icon-edit',
          title: 'Discover',
        },
        {
          icon: 'el-icon-video-camera',
          title: 'Movie',
        },
        {
          icon: 'el-icon-magic-stick',
          title: 'Music',
        },
        {
          icon: 'el-icon-bangzhu',
          title: 'Series',
        },
      ],
      botList: [
        {
          icon: '',
          title: 'Browser',
        },
        {
          icon: 'el-icon-edit',
          title: 'Discover',
        },
        {
          icon: 'el-icon-video-camera',
          title: 'Movie',
        },
        {
          icon: 'el-icon-magic-stick',
          title: 'Music',
        },
        {
          icon: 'el-icon-bangzhu',
          title: 'Series',
        },
      ],
    }
  },
  components: {
    leftBandTop,
    leftBandMid,
    leftBandBot,
  },
}
</script>
<style scoped>
.leftBand {
  height: 100vh;
  background-color: black;
  padding-left: 8%;
}
</style>
