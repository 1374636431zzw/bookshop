<template>
  <div id="Index">
    <div class="swiper">
      <el-carousel indicator-position="outside">
        <el-carousel-item v-for="item in 5" :key="item">
          <h3>{{ item }}</h3>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>
<script>
export default {
  name: "Index"
};
</script>
<style lang="less" scoped>
// 轮播图样式
.el-carousel__item h3 {
    color: #475669;
    font-size: 18px;
    opacity: 0.75;
    line-height: 300px;
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
</style>