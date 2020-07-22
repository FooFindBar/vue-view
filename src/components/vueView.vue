<template>
  <div class="big">
    <div class="main">
      <vueViewItem v-for="(item,index) in list" :obj="item"></vueViewItem>
    </div>
  </div>
</template>

<script>
import vueViewItem from '@/components/vueViewItem.vue'

export default {
  data () {
    return {
      list: [
        {
          imgurl: require('@/assets/img/1.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/2.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/3.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/4.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/5.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/6.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/1.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/2.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/3.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/4.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/5.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/6.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/1.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/2.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/3.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/4.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/5.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
        {
          imgurl: require('@/assets/img/6.jpg'),
          title: '请传入标题',
          desc: '请传入详情',
        },
      ]
    }
  },
  components: {
    vueViewItem
  }
}
</script>

<style scope lang='less'>
@width: 100vw; //控件大小
@height: 100vh; //控件高度
@itemHeight: 45vh; //项高度
.big {
  width: @width;
  height: @height;
  perspective: 100px;
  transform-style: preserve-3d;
  overflow-y: auto;
}

.main {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: @width;
}
.list-item {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
  width: @width;
  height: @itemHeight;
  overflow: hidden;
  background-color: rgba(0, 0, 0, 0.2);
  transition: all 0.3s ease;
  &:hover {
    background-color: rgba(0, 0, 0, 0);
  }
}
// -------------------------------------------滚动条
.big::-webkit-scrollbar {
  /*滚动条整体样式*/
  width: 5px; /*高宽分别对应横竖滚动条的尺寸*/
  height: 1px;
}
.big::-webkit-scrollbar-thumb {
  /*滚动条里面小方块*/
  border-radius: 10px;
  box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.2);
  background: #535353;
}
.big::-webkit-scrollbar-track {
  /*滚动条里面轨道*/
  box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.2);
  border-radius: 10px;
  background: #ededed;
}
</style>


