<template>
  <div class="right-bot">
    <el-row>
      <el-col :span="8">
        <div class="grid-content">
          <div class="right-bot-fir">
            <div>
              <h1>LEFT</h1>
              <img src="../../assets/img/1-5.jpg" alt />
              <div class="span-fir">Almost every child will complain about parents.</div>
              <el-button plain class="btn-fir">朴素按钮</el-button>
            </div>
          </div>
        </div>
      </el-col>
      <el-col :span="16">
        <div class="grid-content">
          <div class="right-bot-sec">
            <div>
              <h1>RIGHT</h1>
              <div
                v-for="(item, index) in botList"
                :key="index"
                class="right-bot-content"
              >
                <el-row class="right-el-row">
                  <el-col :span="6" style="text-align:left">
                    <span>{{ item.title }}</span>
                  </el-col>
                  <el-col :span="6">
                    <span>{{ item.year }}</span>
                  </el-col>
                  <el-col :span="6">
                    <span>
                      <i class="el-icon-user"></i>
                      {{ item.num }}
                    </span>
                  </el-col>
                  <el-col :span="6">
                    <span>
                      <i class="el-icon-view"></i>
                      {{ item.like }}
                    </span>
                  </el-col>
                </el-row>
              </div>
            </div>
          </div>
        </div>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  name: 'rightBandBot',
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
.right-bot {
  height: 55%;
  width: 100%;
  /* background-color: #fff; */
  z-index: 10;
  position: absolute;
  bottom: 0;
  opacity: 0.8;
  filter: drop-shadow(100px -100px 200px black);
}
.right-bot .right-bot-fir {
  width: 70%;
  margin: 0 15%;
  /* background-color: rgb(190, 42, 42); */
}
.right-bot .right-bot-fir h1,
.right-bot .right-bot-sec h1 {
  margin: 0 0 10px 0;
  color: rgb(255, 255, 255);
}
.right-bot .right-bot-fir img {
  width: 90%;
  margin-bottom: 5%;
}
.span-fir {
  color: aliceblue;
  margin-bottom: 5%;
}
.btn-fir {
  width: 90%;
  color: #fff;
  background-color: transparent;
}

.right-bot .right-bot-sec {
  width: 90%;
  margin: 0 3%;
  /* background-color: rgb(156, 18, 18); */
}
.right-bot-sec .right-bot-content {
  height: 10%;
  line-height: 50px;
  font-weight: bolder;
  color: #fff;
  margin-bottom: 3%;
  filter: drop-shadow(5px 5px 10px black);
  text-align: center;
}
.right-bot-sec .right-bot-content .right-el-row {
  opacity: 1;
}
</style>
