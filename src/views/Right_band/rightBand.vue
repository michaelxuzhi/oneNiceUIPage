<template>
  <div class="rightBand">
    <right-band-top></right-band-top>
    <img src="../../assets/img/widthPic.jpg" alt="右大图" />
    <right-band-mid></right-band-mid>
    <right-band-bot :botList="botList"></right-band-bot>
  </div>
</template>
<script>
import rightBandTop from './rightBandTop'
import rightBandBot from './rightBandBot'
import rightBandMid from './rightBandMid'
export default {
  name: 'rightBand',
  data() {
    return {
      botList: [
        {
          title: 'first title',
          year: 2016,
          num: 100000,
          like: 100,
        },
        {
          title: 'second title',
          year: 2016,
          num: 100000,
          like: 100,
        },
        {
          title: 'third title',
          year: 2016,
          num: 100000,
          like: 100,
        },
        {
          title: 'forth title',
          year: 2016,
          num: 100000,
          like: 100,
        },
        {
          title: 'forth title',
          year: 2016,
          num: 100000,
          like: 100,
        },
      ],
    }
  },
  components: {
    rightBandTop,
    rightBandMid,
    rightBandBot,
  },
}
</script>
<style scoped>
.rightBand {
  height: 100vh;
  width: 100%;
  position: relative;
  background-color: rgb(82, 78, 78);
}
.rightBand img {
  height: 100%;
  width: 100%;
  position: abosulte;
  background-size: cover;
  opacity: 0.8;
  filter: alpha(opacity=60);
}
</style>
