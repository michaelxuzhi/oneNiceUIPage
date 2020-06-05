<template>
  <div class="home_big">
    <el-row>
      <el-col :span="5">
        <left-band></left-band>
      </el-col>
      <el-col :span="19">
        <right-band></right-band>
      </el-col>
    </el-row>
  </div>
</template>
<script>
import leftBand from '../views/Left_band/leftBand'
import rightBand from '../views/Right_band/rightBand'
export default {
  name: 'Home',
  data() {
    return {}
  },
  components: {
    leftBand,
    rightBand,
  },
}
</script>
<style scoped></style>
