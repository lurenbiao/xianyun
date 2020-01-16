<template>
  <div>
    <el-carousel height="700px" direction="vertical" :autoplay="true" class="carousel">
      <el-carousel-item v-for="item in imgurl" :key="item" :interval="3500">
       <div class="banner-img" :style="`background:url(${item}) center center no-repeat; background-size: cover;`"></div>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imgurl: [
        "/backiee-125702.jpg",
        "backiee-121981.jpg",
        "backiee-129003.jpg",
        "backiee-129851.jpg"
      ]
    };
  },
  components: {}
};
</script>

<style>
.banner-img{
    height: 700px;
}

</style>