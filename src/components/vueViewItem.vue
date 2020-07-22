<template>
  <section class="list-item">
    <div class="item-image">
      <img :src="obj.imgurl" />
    </div>
    <div class="item-text">
      <div class="item-title">「{{obj.title}}」</div>
      <div class="item-desc">——{{obj.desc}}</div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {

    }
  },
  props: {
    obj: {
      type: Object,
      default: {
        imgurl: '没有图片',
        title: '请传入标题',
        desc: '请传入详情',
        url: ''
      }
    }
  },
  components: {

  }
}
</script>

<style lang='less' scope>
@import url("~@/assets/font/font.css");
.item-image {
  position: absolute;
  width: 100%;
  height: 100%;
  display: block;
  background-color: lightblue;
  transform: translateZ(-60px) scale(2.4);
  z-index: -1;
  img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
.item-text {
  font-family: "si-le";
  text-align: center;
  color: #ffffff;
  .item-title {
    font-size: 2rem;
    font-weight: bold;
    margin-bottom: 20px;
  }
  .item-desc {
    text-align: right;
    font-size: 1.2rem;
  }
}
</style>
