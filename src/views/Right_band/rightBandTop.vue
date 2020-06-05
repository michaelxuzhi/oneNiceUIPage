<template>
  <div class="right-top">
    <el-row>
      <el-col :span="12">
        <div class="grid-content">
          <div class="right-top-fir">
            <el-input class="search" placeholder="请输入内容" prefix-icon="el-icon-search"></el-input>
          </div>
        </div>
      </el-col>
      <el-col :span="12">
        <div class="grid-content">
          <div class="right-top-sec">
            <img class="right-img" src="../../assets/img/1-5.jpg" alt="右头像" />
          </div>
        </div>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  name: "rightBandTop"
};
</script>
<style>
.right-top {
  width: 100%;
  height: 80px;
  z-index: 10;
  position: absolute;
  /* background-color: rgb(116, 12, 12); */
}
.right-top .right-top-fir {
  line-height: 80px;
  padding-left: 50px;
}
.right-top .right-top-fir .el-input__inner {
  width: 60%;
  border-radius: 50px;
  background-color: rgb(88, 85, 85);
  border: none;
  color: #fff;
  height: 35px;
}
.right-top-sec {
  height: 80px;
  /* background-color: rgb(152, 223, 131); */
}
.right-top-sec .right-img {
  padding: 20px;
  float: right;
  height: 40px;
  border-radius: 50%;
}
</style>
