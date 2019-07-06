<template>
  <div class="icons">
    <div class="icon" v-for="item of iconList" :key="item.id">
      <div class="icon-img">
        <img class="icon-img-content" :src="item.imgUrl" alt />
      </div>
      <p class="icon-desc">{{item.name}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeIcons",
  data() {
    return {
      iconList: [
        {
          id: "001",
          imgUrl:
            "http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png",
          name: "景点门票"
        },
        {
          id: "002",
          imgUrl:
            "http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png",
          name: "水上乐园"
        },
        {
          id: "003",
          imgUrl:
            "http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/3ef092d0a89ffddb7f781cda30c8ae49.png",
          name: "暑期大促"
        },
        {
          id: "004",
          imgUrl:
            "http://img1.qunarzz.com/piao/fusion/1803/f5/c4c9d9830404e602.png",
          name: "室内娱乐"
        },
        {
          id: "005",
          imgUrl:
            "http://img1.qunarzz.com/piao/fusion/1803/76/eb88861d78fb9902.png",
          name: "动植物园"
        },
        {
          id: "006",
          imgUrl:
            "http://img1.qunarzz.com/piao/fusion/1803/95/8246f27355943202.png",
          name: "世纪公园"
        },
        {
          id: "007",
          imgUrl:
            "http://img1.qunarzz.com/piao/fusion/1803/47/c2b659e048b11602.png",
          name: "上海野生"
        },
        {
          id: "008",
          imgUrl:
            "http://img1.qunarzz.com/piao/fusion/1803/de/f26be47a6bf02a02.png",
          name: "上海迪士尼"
        }
      ]
    };
  }
};
</script>

<style lang="stylus" scoped>
.icons {
  overflow: hidden;
  width: 100%;
  height: 3.8rem;

  .icon {
    position: relative;
    overflow: hidden;
    float: left;
    width: 25%;
    height: 1.9rem;
    .icon-img {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: .5rem;
        box-sizing: border-box;
        padding: .1rem;
        .icon-img-content {
            display: block;
            margin: 0 auto;
            height: 100%;
        }
    }
    .icon-desc {
        position: absolute;
        left: 0;
        right: 0;
        bottom: 0;
        height: .5rem;
        line-height: .5rem;
        text-align: center;
    }
  }
}
</style>

